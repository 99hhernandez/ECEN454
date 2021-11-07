## 4-bit Adder Schematic Transistor Level
![DataPath](4bitAdder_transistors.png)

## 4-bit Adder Critical Path
![DataPath](4bitAdder_critical.jpg)
![DataPath](4bitAdder_gates.png)

## CALCULATIONS
![img](http://www.sciweavers.org/tex2img.php?eq=C_%7BXOR2%7D%3D7.78fF&bc=Black&fc=White&im=jpg&fs=12&ff=arev&edit=0) <tab> ![img](http://www.sciweavers.org/tex2img.php?eq=C_%7BNAND2%7D%3D2.51fF&bc=Black&fc=White&im=jpg&fs=12&ff=arev&edit=0)

### Path Logical Effort (G)
![img](http://www.sciweavers.org/tex2img.php?eq=G%3D%20%5Cprod%20g_%7Bi%7D%3Dg_%7BXOR2%7D%20%5Cbullet%20%28g_%7BNAND2%7D%29%5E%7B8%7D%3D4%28%5Cfrac%20%7B4%7D%7B3%7D%29%5E%7B8%7D%3D39.95&bc=Black&fc=White&im=jpg&fs=12&ff=arev&edit=0[/img])

### Path Electrical Effort (H)
![img](http://www.sciweavers.org/tex2img.php?eq=H%3D%5Cfrac%7BC_%7Bout-path%7D%7D%7BC_%7Bin-path%7D%7D%3D%5Cfrac%7BC_%7Bload%7D%7D%7BC_%7BXOR2%7D%7D%3D%5Cfrac%20%7B30fF%7D%7BC_%7BXOR2%7D%7D%3D%5Cfrac%20%7B30fF%7D%7B7.78fF%7D%3D3.86&bc=Black&fc=White&im=jpg&fs=12&ff=arev&edit=0)

### Path Branching Effort (B)
![img](http://www.sciweavers.org/tex2img.php?eq=B%3D%20%5Cprod%20b_%7Bi%7D%3D%20%5Cprod%20%5Cfrac%20%7BC_%7Bon-path%7D%2BC_%7Boff-path%7D%7D%7BC_%7Bon-path%7D%7D%3D%20%5Cbig%28%5Cfrac%20%7BC_%7BNAND2%7D%2BC_%7BXOR2%7D%7D%7BC_%7BNAND2%7D%7D%5Cbig%29%5E%7B4%7D%20%5Cbig%28%5Cfrac%20%7BC_%7BNAND2%7D%7D%7BC_%7BNAND2%7D%7D%5Cbig%29%5E%7B4%7D%3D%284.1%5E%7B4%7D%29%281%5E%7B4%7D%29%3D282.6%20&bc=Black&fc=White&im=jpg&fs=12&ff=arev&edit=0[/img])
  
### Stage Effort (\hat{f})
![img](http://www.sciweavers.org/tex2img.php?eq=%20%5Chat%7Bf%7D%3DF%5E%7B%5Cfrac%20%7B1%7D%7BN%7D%7D%3D%28GBH%29%5E%7B%5Cfrac%20%7B1%7D%7BN%7D%7D%3D43578.9%5E%7B%5Cfrac%20%7B1%7D%7B9%7D%7D%3D3.28%20&bc=Black&fc=White&im=jpg&fs=12&ff=arev&edit=0[/img])
