# Line flow module

## Introduction
---
- Ring:bit car V2 line following module is a dedicated module designed for the Ring:bit car V2, it is easy to be installed to achieve the line following function for the Ring:bit car V2. 
- Equipped with double infrared probes, it can detect the distance between 2~12mm accurately that can achieve the function of line following around the circles, the detection of the black lines and the detection of the edge.

 ![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/ring_bit_v2_line_01.jpg)![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/ring_bit_v2_line_02.jpg)

## Features
---
- The micro:bit can drive it directly with the input voltage of this module in 3V~5V.
- It only needs one IO port it with standard 3-pin GVS ports.
- It uses the infrared light to detect with a strong anti-interference capability.

## Parameter
---

 Items | Parameter | Notes 
 :-: | :-: |:-:
 Name |Ring:bit car V2 line following module|-
 SKU|EF03424|-
 Working Voltage |DC 3-5V|-
 Port |Ring:bit car dedicated pin ports|Fixed by screws
 Types of Output Signal |Simulation|-
 Effective Distance |2~12mm|-
 Dimension |34.15 x 27.20mm|-
 Net Weight |4.7g|-


## Dimensions:
---

 ![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/ring_bit_v2_line_03.png)


## Quick to Start
---
### Hardware Connection  
---
- The first step is to insert this module to the baseboard of the Ring:bit car V2.

 ![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/ring_bit_v2_line_04.gif)

- The next step is to fix the module with the two screws.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/ring_bit_v2_line_05.gif) ![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/ring_bit_v2_line_06.gif)

- Completed.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/ring_bit_v2_line_07.jpg)

### Software Programming  
---

- Program a simple line-following code in the [makecode](https://makecode.microbit.org/) .

- Initiate the connection ports for the left and right wheels to P1 and P2.

- When the left detection probe detects deviation from the black line, the right wheel would stop moving and the left wheel would adjust to go back to the black line at the speed of 50.

- The right detection probe would work as the same as the way of the left detection probe works.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/ring_bit_v2_line_08.png)

 Links:[https://makecode.microbit.org/_K0xELbUoeJ2t](https://makecode.microbit.org/_K0xELbUoeJ2t)

You can also download the code directly below:

 <div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_K0xELbUoeJ2t" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### Result
---
- The Ring:bit car runs around the circle slowly.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/ring_bit_v2_line_09.gif)

## FAQ
---
