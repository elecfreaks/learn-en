# Wukong Breakout Board(EF08207)

## Introduction
- - - - -

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_00.jpg)

Wukong is a high integrated breakout board with multiple functions based on micro:bit, which has a similar size with the micro:bit with buzzer, servo and motor drivers on board.

With a built-in 400mAh Li-ion battery pack and the on-board power controlling system, it supports fast charge with only 20 minutes for full filling that can operate for more than 40 minutes a time.

The base board designs with standard 7x5 square bricks that can adapt perfectly to Lego.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_01.jpg)


## Products Link

[Wukong Breakout Board](https://www.elecfreaks.com/wukong-board-with-lego-holder-for-micro-bit.html)

## Characteristics
- - - - -

- Tiny shape with high integration
- Standard Lego bricks connection
- Most of the IO ports led out in GVS form
- Standalone IIC pots, available for OLED and BME280.
- Integrated buzzer and switch
- Integrated motor-drive circuit
- Integrated servo-drive circuit
- Support 5V sensors
- Built-in 400mAh Li-ion battery pack,  on-board power controlling system, four LEDs indicate the power storage
-  Support fast charge


## Parameter
- - - - -

| Parameter | Detail | Instruction | Note |
|:-:|:-:|:-:|:-:|
|Item No.|EF08207|SKU|-|
| Size |40.00 X 58.12 X 24.53 mm|Including Lego baseboard without micro:bit|Manual measure, size in kind prevail|
| Weight |41.6g|Including Lego baseboard and the battery|Manual measure, weight in kind prevail|
| Power Switch |Click to turn on, double to turn off|Four LEDs indicate the power storage, support fast charge|Power supply by the USB connection on board is supported|
| Battery |400mAh Li-ion battery pack|20 minutes for completing the charge that can operate for more than 40 minutes a time|Anti-explosion|
| Working Voltage |3.7v~5v|Li-ion battery pack 3.7v，USB 5v|-|
| Working Temperature |-20℃~60℃|Charge temperature 0℃~40℃|-|
| Motor Drive |Dual (M1，M2)|Motor drive circuit onboard |-|
| Servo Drive |Eight ways servo connection (S0~S7)|Servo drive circuit onboard|-|
| IO Port Lead Out |P0、P1、P2、P8、P12、P13、P14、P15、IIC|Support 3V&5V modules|GVS|
| Rainbow LED |LED0、LED1、LED2、LED3|Available for RainbowLED database|Connect to micro:bit P16 port|
| Buzzer |Passive buzzer with a switch on board|Available for music database|Connect to micro:bit P0 port|
| LED |8 LEDs can be programmed on the base side|Light on, twinkle, breathing light|The LED twinkles when power on| Lego baseboard |Standard 7x5 rectangle base board|Battery is attached in the middle of the baseboard|-|


***Note:*** Any overcharge or over-discharge may result in swelling of the batteries. If your battery is not going to be used for a long time: store it in cool and dry place. Please disconnect your battery with the power source once it is fully charged in case of the overcharge and do not leave it plugged in all the time. *



## Dimmension
- - - - -

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_02.png)


## Introduction to Main Modules
- - - - -

### Power supply, USB power connection and power storage indicating LED

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_07.jpg)

### micro:bit adapter

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_15.jpg)

### Motor-drive connection

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_03.jpg)

### Servo-drive connection

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_04.jpg)

### 8 ways standard GVS connection and 5v connection

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_05.jpg)

### I2C female header conncetion

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_06.jpg)

### 4 Rainbow LEDs

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_08.jpg)

### Buzzer(reverse side) and switch

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_09.jpg)
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_10.jpg)

### 8 LEDs(reverse side)

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_11.jpg)

### Battery connection(reverse side)

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_12.jpg)

### Fixed holes M3 for Lego (reverse side)

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_13.jpg)


## Quick Start
- - - - -

### Hardware Connection

- Insert the micro:bit into the adapter(The logo side of the micro:bit stands towards the side for buzzer switch )
- Click to power on.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_20.jpg)

### Software Programming

- [MicroSoft makecode online programming: makecode.microbit.org](makecode.microbit.org)

### Add Package

- Click `Extensions` in the drawer of `Advanced` to see bricks menu.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot-pk-1.png)

- Search `wukong` in the box and click it to add package.
- Completed

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_14.png)

## User Guide

------

### Ways to power on&charge 

- Original power switch, click to power on and the indicator LED lights on. 
- Double click to power off and the indicator LED lights off. 
- Connect the USB cable to the on-board connection. The normal lighting-on LEDs indicate the state of charge, if the left LEDs lights on in turn, it indicates the charge of the battery. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_07.jpg)

### Breathing LEDs

- There are 8 blue breathing  LEDs whose power on/off status and brightness can be controlled on the baseboard. 

Links: [https://makecode.microbit.org/_4ub57g5FuJ1v](https://makecode.microbit.org/_4ub57g5FuJ1v)；You can also download it below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_4ub57g5FuJ1v" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

### Motor

- There are two kinds of motor driving connections named M1 and M2 that can connect most motors in the market. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_03.jpg)

Links:[https://makecode.microbit.org/_78keCLdmU1Ez](https://makecode.microbit.org/_78keCLdmU1Ez)，You can also download it below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_78keCLdmU1Ez" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

### Buzzer

- There is an on-board buzzer that is connected to the P0 port of the micro:bit, it can be programmed by the `Music` brick and can be powered on/off with the on-board buzzer switch. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_09.jpg)
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_10.jpg)

Links:[https://makecode.microbit.org/_JmM5btU4dHUb](https://makecode.microbit.org/_JmM5btU4dHUb)

You can also download it below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_JmM5btU4dHUb" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

### Rainbow LEDs

- There are 4 Rainbow LEDs named LED0、LED1、LED2、LED3 that are connected to P16 port of the micro:bit and they can be programmed by the  `Neopixel` brick. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_08.jpg)

Links: [https://makecode.microbit.org/_61T2w6cqTib0](https://makecode.microbit.org/_61T2w6cqTib0)

You can also download it below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_61T2w6cqTib0" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

### Servo

- Connect the servos to their driving connections S0~S7, they can be programmed by the servo bricks in Wukong expansions.  
- 180° servos can be set from 0°~180°. 
- Set 0° as the maximum speed of positive rotation, 180° as the maximum speed of negative rotation and 90° as stop for 360° servos , 0°~90° and 90°~180° are the scape for adjusting the speed. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_04.jpg)

Links: [https://makecode.microbit.org/_6Pw63w49u5qq](https://makecode.microbit.org/_6Pw63w49u5qq)

You can also download it below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_6Pw63w49u5qq" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

### 5V Power Supply Pins

- There are 3 pairs on-board 5V power supply connections that can drive sensors or servos in 5V , it only requires to connect the connections for 5V modules to 5V power supply, and to connect the signal cables to the signal connections for servos or sensors. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitExtensionModule/images/wukong_16.png)



- - - - -
