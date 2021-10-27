# !!! GO [HERE](https://github.com/99hhernandez/ECEN454/blob/main/Lab07/Files_Provided/README.md) FOR TYPOS AND CORRECTIONS !!!

## INTRODUCTION
Design Vision is the graphical interface to the Synopsys family of logic synthesis tools. Internally it runs
design compiler. This lab is to familiarize you with the basics of synthesis using Design Vision through a simple
example "cruise control design". After synthesis, you will do pre-layout static timing analysis of your synthesized
design. You will define constraints for your design and check the timing of all the paths in the design. In the final part
of this lab we will use the synthesized Verilog netlist that you will generate for the cruise control logic to "Place and
Route" the circuit on a die.

## PART A: LOGICC SYNTHESIS
In this case we need to synthesize the logic with a certain specific library for 180nm technology. The Synopsys
database format (db) file for a typical 180nm technology is provided. We need to ensure that the
synthesis is performed according to this library file (see below for procedure). What this means is that the optimization
(power, timing, area etc.) will be performed according to the characteristics of the standard cells given in this file.

## PART B: TIMING ANALYSIS
Timing analysis is to check the timing requirement of the circuit. You can do timing analysis at
different design stages - pre-layout with wire-load models or post-layout with actual wires.
PrimeTime® (PT) is the static timing analysis (STA) tool from Synopsys. It is the most widely used
STA engine.
Though Design compiler has its own timing engine, it cannot come close to Primetime's accuracy.
Moreover, primetime can also consider signal integrity effects like coupling noise due to cross talk
and analysis of complex interconnect structures.

## PART C: AUTOMATIC PLACE AND ROUTING
In the previous lab section we generated the synthesized netlist of the cruise control circuit of a vehicle. We now
intend to use this netlist along with the standard cell libraries to place and route the circuit on a die. The same
standard cell library that was used to generate the synthesized netlist will be used here too.
You must observe here that we do not use Custom Layout design as we practiced in the first 6 lab sessions. You will
notice in this lab that the cruise control circuit will use many more standard cells than the 4 bit pipelined adder that you
previously designed. It will be extremely difficult to manually draw the layout and perform routing on the standard cells.
Hence we use a library with predefined standard cells (defined in terms of area, delay and power consumption) to
generate the layout of the circuit by using automatic place and route procedures. The disadvantage with this automatic
flow is that sometimes we do not get the desired level of optimization.

