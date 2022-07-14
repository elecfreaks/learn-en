# Case 05: Automatic Dryer

## Introduction

Put your hands under the air outlet of the automatic hand dryer, it will automatically send out the wind to dehumidify and dry your hands, and then automatically stop the wind and shut down. It can meet the requirements of not using towels to dry hands and preventing cross-infection of diseases. Thus, we can use micro:bit to make an automatic dryer.

![](./images/case_05_01.png)

## Quick Start


### Materials Required

Nezha expansion board × 1

micro:bit × 1

Sonar:bit × 1

Motor × 1

RJ11 wires × 1
***Tips: You may need to purchase [Nezha Inventor's Kit](https://www.elecfreaks.com/nezha-inventor-s-kit-for-micro-bit-without-micro-bit-board.html) if you want all the above compoents.***

### Connection Diagram 

Connect the sonar:bit to J1 and the motor to M1 on the Nezha expansion board as the picture shows.


![](./images/case_05_03.png)

### Assembly Video


Video reference: [https://youtu.be/5kB0bYEsJ1c](https://youtu.be/5kB0bYEsJ1c)


<iframe width="560" height="315" src="https://www.youtube.com/embed/5kB0bYEsJ1c" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


### Assembly Steps


![](./images/case_step_05_01.png)

![](./images/case_step_05_02.png)

![](./images/case_step_05_03.png)

![](./images/case_step_05_04.png)

![](./images/case_step_05_05.png)

![](./images/case_step_05_06.png)

![](./images/case_step_05_07.png)

![](./images/case_step_05_08.png)

![](./images/case_step_05_09.png)

![](./images/case_step_05_10.png)

![](./images/case_step_05_11.png)

![](./images/case_step_05_12.png)



## MakeCode Programming



### Step 1

Click "Advanced" in the MakeCode to see more choices.

![](./images/case_01_10.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "PlanetX" in the dialogue box to download it. 

![](./images/case_01_11.png)



For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "nezha" in the dialogue box to download it. 

![](./images/case_03_09.png)

***Notice:*** If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

### Step 2

### Code as below:

![](./images/case_05_10.png)


### Reference
Link：[https://makecode.microbit.org/_LTA1RLL1ddfM](https://makecode.microbit.org/_LTA1RLL1ddfM)

You may also download it directly below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_LTA1RLL1ddfM" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Result
While there is any object detected by the Sonar:bit, the fan moves automatically. 


![](./images/case-gif-05.gif)
