# Case 36: Color Recognition Password Door

## Introduction 

This is a unique code door because it uses colors as the password. The code door will only open when the color cards are placed in the correct order.

![](./images/case_36_01.png)

## Quick Start 


### Materials Required


Nezha expansion board × 1

micro:bit V2 × 1

color sensor  × 1

Servo  × 1

Crash sensor  × 1

Bricks × n

***Tips: You may need to purchase [Nezha Inventor's Kit](https://www.elecfreaks.com/nezha-inventor-s-kit-for-micro-bit-without-micro-bit-board.html) and [Purchase Interactive coding accessories pack here.](https://www.elecfreaks.com/interactive-coding-accessories-pack.html) if you want all the above components.***



### Connection Diagram 

Inset the micro:bit, connect the color sensor to IIC port, the 360 degrees servo to S1 and the crash sensor to J1 port on Nezha expansion board. 


![](./images/case_36_03.png)



### Assembly Video


Video link: [https://youtu.be/WiSpnc5fPbA](https://youtu.be/WiSpnc5fPbA)

<iframe width="560" height="315" src="https://www.youtube.com/embed/WiSpnc5fPbA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Assembly Steps

![](./images/case_step_36_01.png)

![](./images/case_step_36_02.png)

![](./images/case_step_36_03.png)

![](./images/case_step_36_04.png)

![](./images/case_step_36_05.png)

![](./images/case_step_36_06.png)

![](./images/case_step_36_07.png)

![](./images/case_step_36_08.png)

![](./images/case_step_36_09.png)

![](./images/case_step_36_10.png)

![](./images/case_step_36_11.png)


## MakeCode Programming 



### Step 1


Click "Advanced" in the MakeCode drawer to see more choices. 

![](./images/case_01_10.png)




We need to add a package for programming. Click "Extensions" in the bottom of the drawer and search with "nezha" to download it. 

![](./images/case_03_09.png)

***Note:*** If you met a tip indicating the codebase might be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

### Step 2

### Programme as the pictures indicate


![](./images/case_36_10.png)



### Reference

Link: [https://makecode.microbit.org/_3xJgWP2ig48r](https://makecode.microbit.org/_3xJgWP2ig48r)

You may download it directly below: 

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_3xJgWP2ig48r" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Result
Sending the passwords via the colors, press the crash sensor to confirm after you choose the colors ready, the door would open if the two passwords are correct or the micro:bit displays "x" and the program reruns. 

![](./images/case-gif-36.gif)
