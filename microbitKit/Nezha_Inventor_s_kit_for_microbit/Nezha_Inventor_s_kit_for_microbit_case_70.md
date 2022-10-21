# Case 70: Voice Controlled Laser Launching Vehicle

## Introduction

Lasers have many applications in daily life, such as laser scalpels in medicine, cutting materials in industry, laser welding and laser drilling. In this lesson, we will experience the fascination of laser by using the laser module, let's start!

![](./images/70_1.png)

### Materials Required

Nezha expansion board × 1

micro:bit V2 × 1

Speech recognition module × 1

Laser module × 1

[Four-Channel Tracking  Sensor](https://shop.elecfreaks.com/products/elecfreaks-planetx-4-channel-tracking-sensor) × 1

Motors × 2

RJ11 cables × 1

Bricks × n

**Note: If you want all of the above components, you may purchase the [Nezha 48 IN 1 Inventor's Kit](https://shop.elecfreaks.com/products/elecfreaks-micro-bit-nezha-48-in-1-inventors-kit-without-micro-bit-board?_pos=3&_sid=7e0550154&_ss=r)**.



### Assembly Steps

Component Details

![](./images/70_2.png)

Build it as the assembly steps suggest:

![](./images/70_3.png)

![](./images/70_4.png)

![](./images/70_5.png)

![](./images/70_6.png)

![](./images/70_7.png)

![](./images/70_8.png)

![](./images/70_9.png)

![](./images/70_10.png)

![](./images/70_11.png)

![](./images/70_12.png)

![](./images/70_13.png)

![](./images/70_14.png)

![](./images/70_15.png)

![](./images/70_16.png)

![](./images/70_17.png)

![](./images/70_18.png)

![](./images/70_19.png)

![](./images/70_20.png)

![](./images/70_21.png)

![](./images/70_22.png)

![](./images/70_23.png)

![](./images/70_24.png)

Completed picture：

![](./images/70_25.png)

## Connection Diagram

We connect the four line following sensor and the speech recognition sensor to the IIC interfaces, the laser module to the J1 interface, and the connection diagram is as follows:

![](./images/70_26.png)


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

![](./images/70_27.png)

Link: https://makecode.microbit.org/_UY7eL28g4h34

You may also download it directly:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_UY7eL28g4h34" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### Result

When we say line following mode, the car will follow the black line on the map. When we say fire laser, the laser module will fire the laser. When we say stop firing, the laser module will stop firing the laser.

![](./images/70_28.gif)
