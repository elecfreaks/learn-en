# Case 31: The Rotary Password Door

## Introduction

The selected password can be adjusted by the potentiometer and confirmed by the crash sensor. If two consecutive passwords are entered within the correct range, the password door will open. Perhaps we can use this device to make some decryption plots to make the game more interesting.

![](./images/case_31_01.png)

## Quick Start 



### Materials Required


Nezha expansion board × 1

micro:bit V2 × 1

Trimpot × 1 

Servo  × 1

Crash sensor  × 1

OLED display  × 1 （It requires to be purchased as standalones.）

Bricks × n

***Tips: You may need to purchase [Nezha Inventor's Kit](https://shop.elecfreaks.com/products/elecfreaks-micro-bit-nezha-48-in-1-inventors-kit-without-micro-bit-board?_pos=2&_sid=ed1b6fbd2&_ss=r) and [Purchase Interactive coding accessories pack here.](https://shop.elecfreaks.com/products/elecfreaks-interactive-coding-accessories-pack?_pos=1&_sid=c75dad35f&_ss=r) if you want all the above components.***




### Connection Diagram 

Inset the micro:bit, connect the OLED display to IIC port, the servo to S1, the trimpot to J1and the crash sensor to J2 on Nezha expansion board. 


![](./images/case_31_03.png)



### Assembly Video


Video link: [https://youtu.be/eniQAfqXym0](https://youtu.be/eniQAfqXym0)

<iframe width="560" height="315" src="https://www.youtube.com/embed/eniQAfqXym0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Assembly Steps

![](./images/case_step_31_01.png)

![](./images/case_step_31_02.png)

![](./images/case_step_31_03.png)

![](./images/case_step_31_04.png)

![](./images/case_step_31_05.png)

![](./images/case_step_31_06.png)

![](./images/case_step_31_07.png)

![](./images/case_step_31_08.png)

![](./images/case_step_31_09.png)

![](./images/case_step_31_10.png)



## MakeCode Programming 



### Step 1


Click "Advanced" in the MakeCode drawer to see more choices. 

![](./images/case_01_10.png)




We need to add a package for programming. Click "Extensions" in the bottom of the drawer and search with "nezha" to download it. 

![](./images/case_03_09.png)

***Note:*** If you met a tip indicating the codebase might be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

### Step 2



### Programme as the pictures indicate


![](./images/case_31_10.png)



### Reference

Link: [https://makecode.microbit.org/_Hc8CCTAUFXv9](https://makecode.microbit.org/_Hc8CCTAUFXv9)

You may download it directly below: 

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Hc8CCTAUFXv9" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Result
Adjust the numbers by rotating the trimpot, press the crash sensor after you choose the numbers ready, the door would open if the two passwords are in the correct ranges or the micro:bit displays "x" and the program reruns. 

![](./images/case-gif-31.gif)

