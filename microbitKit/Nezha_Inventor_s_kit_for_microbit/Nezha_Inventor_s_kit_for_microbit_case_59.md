# Case 59: Submarines

## Introduction

We have seen submarines on TV news or internet pages, and submarines are broadly divided into nuclear-powered and conventional-powered submarines. We know that the technology used in submarines is very diverse and advanced, reflecting the comprehensive technology and economic strength of a country. Of course, there are also submarines used for scientific exploration of the ocean, so let's make a submarine for ocean exploration in this lesson.

![](./images/59_1.jpg)

### Materials Required

Nezha expansion board × 1

micro:bit V2 × 1

Ultrasonic Sound Sensor × 1

Motors × 2

RJ11 cable × 1

Bricks × n

**Note: If you want all of the above components, you may purchase the [Nezha 48 IN 1 Inventor's Kit](https://www.elecfreaks.com/nezha-inventor-s-kit-for-micro-bit-without-micro-bit-board.html)**.



### Assembly Steps

Component Details

![](./images/59_2.jpg)

Build it as the assembly steps suggest:

![](./images/59_3.jpg)

![](./images/59_4.jpg)

![](./images/59_5.jpg)

![](./images/59_6.jpg)

![](./images/59_7.jpg)

![](./images/59_8.jpg)

![](./images/59_9.jpg)

![](./images/59_10.jpg)

![](./images/59_11.jpg)

![](./images/59_12.jpg)

![](./images/59_13.jpg)

![](./images/59_14.jpg)

![](./images/59_15.jpg)

![](./images/59_16.jpg)

![](./images/59_17.jpg)

![](./images/59_18.jpg)

![](./images/59_19.jpg)

![](./images/59_20.jpg)

![](./images/59_21.jpg)

![](./images/59_22.jpg)

![](./images/59_23.jpg)

![](./images/59_24.jpg)

![](./images/59_25.jpg)

![](./images/59_26.jpg)

## Connection Diagram

Connect the four motors to the M1, and M4. and Connect the ultrasonic sensor to the J1

![](./images/59_27.jpg)


##  MakeCode Programming

### Step 1

Click “Advanced” in the MakeCode drawer to see more choices.



![](./images/49_10.png)



For programming the servo, we need to add a package. Click “Extensions” at the bottom of the drawer and search with “nezha” to download it.



![](./images/49_11.png)



For programming the PIR sensor, we need to add a package. Search with “PlanetX” in the dialogue box and click to download it.

![](./images/49_12.png)



*Notice*: If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu.

### Reference

The program is shown below:

![](./images/59_28.jpg)

Link:  https://makecode.microbit.org/_hLPTR36MJCrE

You may also download it directly:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_hLPTR36MJCrE" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### Result

As we can see, the submarine will move forward at a constant speed when there are no rocks in the way, back up when there is an obstacle in front of it, and then move forward again. Of course, you can also improve the program to achieve the submarine trajectory we see in real life.

![](./images/59_29.gif)
