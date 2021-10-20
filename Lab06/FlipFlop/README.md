## SCHEMATIC
![DataPath](DFF_schem.png)

## LAYOUT
![DataPath](DFF_layout.png)

## LVS
```
@(#)$CDS: LVS version 6.1.8-64b 08/04/2020 19:19 (cpgsrv11) $

Command line: /opt/coe/cadence/IC618/tools.lnx86/dfII/bin/64bit/LVS -dir /home/ugrads/h/hernandezh99/cadence/LVS -l -s -t /home/ugrads/h/hernandezh99/cadence/LVS/layout /home/ugrads/h/hernandezh99/cadence/LVS/schematic
Like matching is enabled.
Net swapping is enabled.
Using terminal names as correspondence points.
Compiling Diva LVS rules...

    Net-list summary for /home/ugrads/h/hernandezh99/cadence/LVS/layout/netlist
       count
        13              nets
        6               terminals
        10              pmos
        10              nmos

    Net-list summary for /home/ugrads/h/hernandezh99/cadence/LVS/schematic/netlist
       count
        13              nets
        6               terminals
        10              pmos
        10              nmos


    Terminal correspondence points
    N10       N3        CLK
    N11       N12       D
    N7        N11       GND
    N8        N8        Q
    N12       N7        VDD
    N9        N6        _CLK

Devices in the netlist but not in the rules:
        pcapacitor
Devices in the rules but not in the netlist:
        cap nfet pfet nmos4 pmos4

The net-lists match.

                             layout  schematic
                                instances
        un-matched              0       0      
        rewired                 0       0      
        size errors             0       0      
        pruned                  0       0      
        active                  20      20     
        total                   20      20     

                                  nets
        un-matched              0       0      
        merged                  0       0      
        pruned                  0       0      
        active                  13      13     
        total                   13      13     

                                terminals
        un-matched              0       0      
        matched but
        different type          0       0      
        total                   6       6      


Probe files from /home/ugrads/h/hernandezh99/cadence/LVS/schematic

devbad.out:

netbad.out:

mergenet.out:

termbad.out:

prunenet.out:

prunedev.out:

audit.out:


Probe files from /home/ugrads/h/hernandezh99/cadence/LVS/layout

devbad.out:

netbad.out:

mergenet.out:

termbad.out:

prunenet.out:

prunedev.out:

audit.out:
```
