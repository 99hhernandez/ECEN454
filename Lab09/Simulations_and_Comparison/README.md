### Non-Optimized 4-bit Adder Delays
| Case | Pin | Rising (ps) | Falling (ps) |
| :---: | :---: | :---: | :---: |
| A=0000 B=1111 Carry In=1| SUM[0] | 430.5 | 438.6 |
|  | SUM[1] | 672.8 | 672.7 |
|  | SUM[2] | 937 | 932 |
|  | SUM[3] | 1182 | 1172 |
|  | CARRY | 1175 | 1191 |
| A=1010 B=0101 Carry In=0 | SUM[0] | 434.7 | 437.4 |
|  | SUM[1] | 680.6 | 671.5 |
|  | SUM[2] | 946.8 | 930.6 |
|  | SUM[3] | 1194 | 1171 |
|  | CARRY | 1174 | 1198 |
| A=1010 B=0101 Carry In=1 | SUM[0] | 496.4 | 438.6 |
|  | SUM[1] | 672.9 | 672.5 |
|  | SUM[2] | 937.3 | 932.2 |
|  | SUM[3] | 1183 | 1172 |
|  | CARRY | 1175 | 1191 |
| A=1100 B=1000 Carry In=0 | SUM[0] | 496.4 | 470.8 |
|  | SUM[1] | 773.4 | 732.9 |
|  | SUM[2] | 687.9 | 732.9 |
|  | SUM[3] | 1029 | 958 |
|  | CARRY | 475.7 | 422.2 |

### Optimized 4-bit Adder Delays
| Case | Pin | Rising (ps) | Falling (ps) |
| :---: | :---: | :---: | :---: |
| A=0000 B=1111 Carry In=1| SUM[0] | 419.9 | 430.2 |
|  | SUM[1] | 620.4 | 619.4 |
|  | SUM[2] | 828.5 | 808.9 |
|  | SUM[3] | 1059 | 1025 |
|  | CARRY | 840.3 | 908.6 |
| A=1010 B=0101 Carry In=0 | SUM[0] | 424.1 | 435.4 |
|  | SUM[1] | 625.4 | 618.4 |
|  | SUM[2] | 834.4 | 806.9 |
|  | SUM[3] | 1066 | 1022 |
|  | CARRY | 836.4 | 910.1 |
| A=1010 B=0101 Carry In=1 | SUM[0] | 419.9 | 430.2 |
|  | SUM[1] | 620.6 | 619.6 |
|  | SUM[2] | 828.7 | 809.2 |
|  | SUM[3] | 1059 | 1025 |
|  | CARRY | 840.5 | 908.8 |
| A=1100 B=1000 Carry In=0 | SUM[0] | 476.6 | 470.2 |
|  | SUM[1] | 674.0 | 637.2 |
|  | SUM[2] | 599.4 | 629.7 |
|  | SUM[3] | 881.3 | 871.8 |
|  | CARRY | 289.9 | 233.2 |
  
  
### Power Dissipation
| Case | Non-Optimized (μW) | Optimized (μW) |
| :---: | :---: | :---: |
| A=0000 B=1111 Carry In=1 | -115.8 | -113.0 |
| A=1010 B=0101 Carry In=0 | -115.7 | -113.0 |
| A=1010 B=0101 Carry In=1 | -115.7 | -113.1 |
| A=1100 B=1000 Carry In=0 | -119.1 | -115.1 |


### Area
| Non-Optimized (μm<sup>2</sup>) | Optimized (μm<sup>2</sup>) |
| :---: | :---: |
| 18 | 19.84 |

  Non-Optimized:
  <br>![img](http://www.sciweavers.org/tex2img.php?eq=%20Area%3D8Area_%7BXOR2%7D%20%2B%2012Area_%7BNAND2%7D&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0)
  <br>![img](http://www.sciweavers.org/tex2img.php?eq=%20Area%3D8%281.68%20%5Cmu%20m%5E%7B2%7D%29%20%2B%2012%280.38%20%5Cmu%20m%5E%7B2%7D%29&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0)

  Optimized:
  <br>![img](http://www.sciweavers.org/tex2img.php?eq=%20Area%3D8Area_%7BXOR2%7D%2B10Area_%7BNAND2%7D%2BArea_%7BNAND2_%7Bg8%7D%7D%2BArea_%7BNAND2_%7Bg9%7D%7D&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0)
  <br>![img](http://www.sciweavers.org/tex2img.php?eq=Area%3D8%281.68%20%5Cmu%20m%5E%7B2%7D%29%2B10%280.38%20%5Cmu%20m%5E%7B2%7D%29%2B%280.76%20%5Cmu%20m%5E%7B2%7D%29%2B%281.84%20%5Cmu%20m%5E%7B2%7D%29&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0)
