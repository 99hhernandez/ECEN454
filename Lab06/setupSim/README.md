## SCHEMATIC
![DataPath](DFF_setuptime_schem.png)

## SETUP TIME

#### SETUP RISE
![DataPath](setup_rise.png)

#### SETUP FALL
![DataPath](setup_fall.png)

setup_rise = CLK_rise - Q_rise = 10 - 9.85 = 0.15ns

setup_fall = CLK_fall - Q_fall = 20 - (10 + 9.73) = 0.27ns

setup_fall > setup_rise --> setup time = 0.27ns
