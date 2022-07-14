# Case 02: Flower-watering Prompter

## Introduction

Some plants can make people live healthier. For example, a pot of green dill in a room of 8-10 square meters is equivalent to an air purifier, which can effectively absorb harmful gases such as formaldehyde, benzene and trichloroethylene in the air. Thus, we can make a simple watering device to help us take care of plants.

![](./images/case_02_01.png)

## Quick Start

### Materials Required 

Nezha expansion board × 1

micro:bit × 1

LED-red × 1

LED-green × 1

Soil moisture sensor × 1

RJ11 wires × 3

***Tips: You may need to purchase [Nezha Inventor's Kit](https://www.elecfreaks.com/nezha-inventor-s-kit-for-micro-bit-without-micro-bit-board.html) if you want all the above compoents.***



### Connection Diagram 

Connect the green LED to J4, red LED to J3 and soil moisture sensor to J2 on the Nezha expansion board as the picture shows.


![](./images/case_02_03.png)


### Assembly Video

Video reference:[https://youtu.be/YxEKEoDB6FQ](https://youtu.be/YxEKEoDB6FQ)


<iframe width="560" height="315" src="https://www.youtube.com/embed/YxEKEoDB6FQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Assembly Steps




![](./images/case_step_02_01.png)

![](./images/case_step_02_02.png)

![](./images/case_step_02_03.png)

![](./images/case_step_02_04.png)

![](./images/case_step_02_05.png)

![](./images/case_step_02_06.png)

![](./images/case_step_02_07.png)

![](./images/case_step_02_08.png)





## MakeCode Programming



### Step 1
Click "Advanced" in the MakeCode to see more choices.

![](./images/case_01_10.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "PlanetX" in the dialogue box to download it. 

![](./images/case_01_11.png)

***Notice:*** If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

### Step 2

### Code as below:

![](./images/case_02_10.png)


### Reference
Link：[https://makecode.microbit.org/_2FgMYuLiUeE8](https://makecode.microbit.org/_2FgMYuLiUeE8)

You may also download it directly below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_2FgMYuLiUeE8" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Result
The red LED lights on for reminding of watering if the soil moisture sensors gets a low value from the earth, or the green LED lights on. 


![](./images/case-gif-02.gif)

