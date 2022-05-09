# Case 15: Volume Reminder 

## Introduction 
---
This device uses the sound intensity detection on the micro:bit V2 to control the servo to rotate to the corresponding position by detecting the surrounding sound level, so that the pointer connected to the servo fluctuates with the volume.

![](./images/case_15_01.png)

## Quick to Start
---

### Materials 

Nezha expansion board × 1

micro:bit × 1

servo  × 1

RJ11 wires × 1

Bricks × n


### Connection Diagram 

Connect the 360 degrees servo to S1 port on the Nezha expansion board. 


![](./images/case_15_03.png)


### Assembly Video

Video link:[https://youtu.be/sq4fq4W51Ck](https://youtu.be/sq4fq4W51Ck)

<iframe width="560" height="315" src="https://www.youtube.com/embed/sq4fq4W51Ck" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


### Assembly Steps


![](./images/case_step_15_01.png)

![](./images/case_step_15_02.png)

![](./images/case_step_15_03.png)

![](./images/case_step_15_04.png)

![](./images/case_step_15_05.png)

![](./images/case_step_15_06.png)

![](./images/case_step_15_07.png)




## MakeCode Programming 
---


### Step 1


Click "Advanced" in the MakeCode drawer to see more choices. 

![](./images/case_01_10.png)

We need to add a package for programming. Click "Extensions" in the bottom of the drawer and search with "PlanetX" to download it. 

![](./images/case_01_11.png)

We need to add a package for programming. Click "Extensions" in the bottom of the drawer and search with "Nezha" to download it. 

![](./images/case_03_09.png)

***Note:*** If you met a tip indicating the codebase might be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

### Step 2


### Programme as the pictures indicate

![](./images/)

![](./images/case_15_15.png)



### Link
Link: [https://makecode.microbit.org/_JfDgxzJkc72X](https://makecode.microbit.org/_JfDgxzJkc72X)

You may download it directly below: 

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_JfDgxzJkc72X" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Result
The servos drive in accordance with the change of the volume. 

![](./images/case-gif-15.gif)
