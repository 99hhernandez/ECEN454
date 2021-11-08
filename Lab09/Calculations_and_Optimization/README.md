## 4-bit Adder Schematic Transistor Level
![DataPath](4bitAdder_transistors.png)

## 4-bit Adder Critical Path
![DataPath](4bitAdder_critical.jpg)
![DataPath](4bitAdder_gates.png)

## CALCULATIONS
![img](https://latex.codecogs.com/png.image?%5Cdpi%7B150%7D%20%5Cbg_black%20C_%7BXOR2%7D=7.78fF)
![img](https://latex.codecogs.com/png.image?%5Cdpi%7B150%7D%20%5Cbg_black%20C_%7BNAND2%7D=2.51fF)
<br>Capacitance of [XOR2 gate](https://github.com/99hhernandez/ECEN454/tree/main/Lab03/XOR2) and [NAND2 gate](https://github.com/99hhernandez/ECEN454/tree/main/Lab03/NAND2) come from the calculated values from Lab 3.

### Path Logical Effort (G)
![G](https://latex.codecogs.com/png.image?%5Cdpi%7B150%7D%20%5Cbg_black%20G=%5Cprod%20g_%7Bi%7D=g_%7BXOR2%7D%5Ctimes%20(g_%7BNAND2%7D)%5E%7B8%7D=4%5Cbig(%5Cfrac%7B4%7D%7B3%7D%5Cbig)%5E%7B8%7D=39.95)
<br>The logical effort of a gate with given inputs can be found on Table 1.1 in Page 7 [here](https://my.eng.utah.edu/~cs6710/handouts/Sutherland_Ch1.pdf).

### Path Electrical Effort (H)
![H](https://latex.codecogs.com/png.image?%5Cdpi%7B150%7D%20%5Cbg_black%20H=%5Cfrac%20%7BC_%7Bout-path%7D%7D%7BC_%7Bin-path%7D%7D=%5Cfrac%20%7BC_%7Bload%7D%7D%7BC_%7BXOR2%7D%7D=%5Cfrac%20%7B30fF%7D%7B7.78fF%7D=3.86)

### Path Branching Effort (B)
![B](https://latex.codecogs.com/png.image?%5Cdpi%7B150%7D%20%5Cbg_black%20B=%5Cprod%20b_%7Bi%7D=%5Cprod%20%5Cfrac%7BC_%7Bon-path%7D&plus;C_%7Boff-path%7D%7D%7BC_%7Bon-path%7D%7D=%5Cbig(%5Cfrac%20%7BC_%7BNAND2%7D&plus;C_%7BXOR2%7D%7D%7BC_%7BNAND2%7D%7D%5Cbig)%5E%7B4%7D%20%5Cbig(%5Cfrac%7BC_%7BNAND2%7D%7D%7BC_%7BNAND2%7D%7D%5Cbig)%5E%7B4%7D=(4.1%5E%7B4%7D)(1%5E%7B4%7D)=282.6)
  
### Stage Effort (\hat{f})
![imgf](https://latex.codecogs.com/png.image?%5Cdpi%7B150%7D%20%5Cbg_black%20%20%5Chat%7Bf%7D=F%5E%7B%5Cfrac%20%7B1%7D%7BN%7D%7D=(GBH)%5E%7B%5Cfrac%20%7B1%7D%7BN%7D%7D=43578.9%5E%7B%5Cfrac%20%7B1%7D%7B9%7D%7D=3.28%20) 

### Transistor Resizing
If 2.7 <= f/hat <= 4, great, if not then you need to change B by resizing gates outside the critical path. If your f/hat falls within range, then start from the end of the critical path and calculate C<sub>in,i</sub> for each gate, making your way to the beginning of the critical path. If your C<sub>in,i</sub> <= C<sub>gate</sub>, dont resize, else resize the transistors by the multiplier you get from C<sub>in,i</sub> / C<sub>gate</sub>.

![Cini](https://latex.codecogs.com/png.image?%5Cdpi%7B150%7D%20%5Cbg_black%20C_%7Bin,i%7D=%5Cfrac%20%7Bg_%7Bi%7DC_%7Bout,i%7D%7D%7B%5Chat%7Bf%7D%7D)
