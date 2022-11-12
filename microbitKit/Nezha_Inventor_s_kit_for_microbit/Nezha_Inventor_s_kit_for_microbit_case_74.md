# Case 74: The Happy Crab

## Introduction

Whenever we think of a crab we think of its horizontal stride and we often see them in funny videos, in this course let's make a happy crab. We will use the RFID sensor as a switch, and when the RFID sensor detects the card, the little crab starts to play happily.

![](./images/74_1.png)

### Materials Required

Nezha expansion board × 1

micro:bit V2 × 1

Servos × 2

RFID Sensor × 1

Motors × 2

RJ11 cables × 1

Bricks × n

**Note: If you want all of the above components, you may purchase the [Nezha 48 IN 1 Inventor's Kit](https://shop.elecfreaks.com/products/elecfreaks-micro-bit-nezha-48-in-1-inventors-kit-without-micro-bit-board?_pos=3&_sid=7e0550154&_ss=r)**.



### Assembly Steps

Components Details

![](./images/74_2.png)

Build it as the assembly steps suggest:

![](./images/74_3.png)

![](./images/74_4.png)

![](./images/74_5.png)

![](./images/74_6.png)

![](./images/74_7.png)

![](./images/74_8.png)

![](./images/74_9.png)

![](./images/74_10.png)

![](./images/74_11.png)

![](./images/74_12.png)

![](./images/74_13.png)

![](./images/74_14.png)

![](./images/74_15.png)

![](./images/74_16.png)

![](./images/74_17.png)

![](./images/74_18.png)

## Connection Diagram

We need to connect the Motors to the M1 and M4 port, the Servos to the S1 and S4 port, and the RFID sensor to the IIC port.

![](./images/74_19.png)


##  MakeCode Programming

### Step 1

Click “Advanced” in the MakeCode drawer to see more choices.



![](./images/49_10.png)



We need to add a package for programming. Click “Extensions” at the bottom of the drawer and search with “nezha” to download it.



![](./images/49_11.png)



We need to add a package for programming. Search with “PlanetX” in the dialogue box and click to download it.

![](./images/49_12.png)



*Notice*: If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu.

### Reference

The program is displayed below:

![](./images/74_20.png)

Link: https://makecode.microbit.org/_Tvxc9aDKb4sW

You may also download it directly:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Tvxc9aDKb4sW" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### Result

When we put the card on the front of the RFID sensor, and the RFID sensor detects the card, the crab will start running sideways and swinging its two pincers in a circular motion.

![](./images/74_21.gif)
