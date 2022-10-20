# Case 11: Line-tracking Car

## Introduction

This is a line tracking car, we can use black electrical tape to paste a track on the white plane, and then make the car drive according to the preset trajectory.

![](./images/case_11_01.png)

## Quick Start

### Materials Required

Nezha expansion board × 1

micro:bit × 1

Line-tracking sensor × 1

Motors × 2

RJ11 wires × 1

***Tips: You may need to purchase [Nezha Inventor's Kit](https://www.elecfreaks.com/nezha-inventor-s-kit-for-micro-bit-without-micro-bit-board.html) if you want all the above compoents.***

### Connection Diagram 
Connect the line-tracking sensor to J1, the two motors to M1&M4 on the Nezha expansion board as the picture shows.


![](./images/case_11_04.png)


** 在搭建过程中需要注意巡线探头离地高度应该为8~11mm，请根据实际情况进行调整。**


### Assembly Steps

![](./images/case_step_11_01.png)

![](./images/case_step_11_02.png)

![](./images/case_step_11_03.png)

![](./images/case_step_11_04.png)

![](./images/case_step_11_05.png)

![](./images/case_step_11_06.png)

![](./images/case_step_11_07.png)

![](./images/case_step_11_08.png)

![](./images/case_step_11_09.png)

![](./images/case_step_11_10.png)

![](./images/case_step_11_11.png)

![](./images/case_step_11_12.png)

![](./images/case_step_11_13.png)

![](./images/case_step_11_14.png)

![](./images/case_step_11_15.png)

![](./images/case_step_11_16.png)

![](./images/case_step_11_17.png)

![](./images/case_step_11_18.png)

![](./images/case_step_11_19.png)

![](./images/case_step_11_20.png)

![](./images/case_step_11_21.png)


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

![](./images/case_11_15.png)



### Reference
Link：[https://makecode.microbit.org/_MbaX4mTEmHmf](https://makecode.microbit.org/_MbaX4mTEmHmf)

You may also download it directly below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_MbaX4mTEmHmf" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Result
The car drives along with the black line. 

![](./images/case-gif-11.gif)
