# Case 09: Invading Detection Device

## Introduction

This is an intrusion detection device. When the ultrasonic sensor detects that someone is approaching, it will automatically turn on a red light and alarm through the buzzer on the micro:bit. If the ultrasonic sensor does not detect anyone, it will automatically turn on green light.

![](./images/case_09_01.png)

## Quick Start



### Materials Required

Nezha expansion board × 1

micro:bit × 1

LED-green × 1

LED-red × 1

Sonar:bit × 1

RJ11 wires × 3



### Connection Diagram 

Connect the sonar:bit to J1, red LED to J2 and green LED to J3 on the Nezha expansion board as the picture shows.


![](./images/case_09_03.png)

### Assembly Video


Video Reference: [https://youtu.be/jw9_wlNIiHw](https://youtu.be/jw9_wlNIiHw)


<iframe width="560" height="315" src="https://www.youtube.com/embed/jw9_wlNIiHw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


### Assembly Steps


![](./images/case_step_09_01.png)

![](./images/case_step_09_02.png)

![](./images/case_step_09_03.png)

![](./images/case_step_09_04.png)

![](./images/case_step_09_05.png)

![](./images/case_step_09_06.png)

![](./images/case_step_09_07.png)

![](./images/case_step_09_08.png)

![](./images/case_step_09_09.png)



## MakeCode Programming




### Step 1

Click "Advanced" in the MakeCode to see more choices.

![](./images/case_01_10.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "PlanetX" in the dialogue box to download it. 

![](./images/case_01_11.png)

Notice: If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

### Step 2

### Code as below:

![](./images/case_09_08.png)


### Reference
Link：[https://makecode.microbit.org/_2zrE6AKRHbqW](https://makecode.microbit.org/_2zrE6AKRHbqW)

You may also download it directly below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_2zrE6AKRHbqW" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  
---

### Result
While the sonar:bit detects the object, the red LED lights up and the buzzer alarms. 

![](./images/case-gif-09.gif)
