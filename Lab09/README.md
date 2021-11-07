## INTRODUCTION
In this lab you have to identify the critical path in your design (4 bit adder), and reduce the
delay of this path by determining the optimal number of devices and sizes of the gates that lie
along this path. You have to use the Logical Effort and Gate sizing techniques you learn in the
course.

## REPORT REQUIREMENTS
1) Print out the schematic of your circuit and __draw a line along the critical path__. Include your
calculations to determine the number of stages in the circuit, the path effort, and the transistor
sizes. You need to __clearly show your calculation steps__. If you wrote a spice netlist, include a
drawing of the critical path.

2) Turn in the waveforms for __the following input vectors:__
    ```
    A=0000, B=1111, CarryIn=1
    A=1010, B=0101, CarryIn=0
    A=1010, B=0101, CarryIn=1
    A=1100, B=1000, CarryIn=0
    ```
    And complete the __table comparing__ the __delays__ and the __VDD Power consumption__ of __both__ the __non-optimized__ and the
__optimized__ circuits for all cases (you need to calculate improvement). Please switch all inputs at the same time as you did in the lab 5.

    Non-Optimized 4-bit Adder Delays:
    | Case | Pin | Rising (ps) | Falling (ps) |
    | :---: | :---: | :---: | :---: |
    | A=0000 B=1111 Carry In=1| SUM[0] |  |  |
    |  | SUM[1] |  |  |
    |  | SUM[2] |  |  |
    |  | SUM[3] |  |  |
    |  | CARRY |  |  |
    | A=1010 B=0101 Carry In=0 | SUM[0] |  |  |
    |  | SUM[1] |  |  |
    |  | SUM[2] |  |  |
    |  | SUM[3] |  |  |
    |  | CARRY |  |  |
    | A=1010 B=0101 Carry In=1 | SUM[0] |  |  |
    |  | SUM[1] |  |  |
    |  | SUM[2] |  |  |
    |  | SUM[3] |  |  |
    |  | CARRY |  |  |
    | A=1100 B=1000 Carry In=0 | SUM[0] |  |  |
    |  | SUM[1] |  |  |
    |  | SUM[2] |  |  |
    |  | SUM[3] |  |  |
    |  | CARRY |  |  |

    Optimized 4-bit Adder Delays:
    | Case | Pin | Rising (ps) | Falling (ps) |
    | :---: | :---: | :---: | :---: |
    | A=0000 B=1111 Carry In=1| SUM[0] |  |  |
    |  | SUM[1] |  |  |
    |  | SUM[2] |  |  |
    |  | SUM[3] |  |  |
    |  | CARRY |  |  |
    | A=1010 B=0101 Carry In=0 | SUM[0] |  |  |
    |  | SUM[1] |  |  |
    |  | SUM[2] |  |  |
    |  | SUM[3] |  |  |
    |  | CARRY |  |  |
    | A=1010 B=0101 Carry In=1 | SUM[0] |  |  |
    |  | SUM[1] |  |  |
    |  | SUM[2] |  |  |
    |  | SUM[3] |  |  |
    |  | CARRY |  |  |
    | A=1100 B=1000 Carry In=0 | SUM[0] |  |  |
    |  | SUM[1] |  |  |
    |  | SUM[2] |  |  |
    |  | SUM[3] |  |  |
    |  | CARRY |  |  |

    Power Consumption:
    | Case | Optimized (uW) | Non-optimized (uW) |
    | :---: | :---: | :---: |
    | A=0000 B=1111 Carry In=1 |  |  |
    | A=1010 B=0101 Carry In=0 |  |  |
    | A=1010 B=0101 Carry In=1 |  |  |
    | A=1100 B=1000 Carry In=0 |  |  |

3) Make a __table comparing the Area__ (sum of all the transistors’ W*L).
   
   Area:
   | Optimized (u^2 m^2) | Non-optimized (u^2 m^2) |
   | :---: | :---: |
   |  |  |
   
