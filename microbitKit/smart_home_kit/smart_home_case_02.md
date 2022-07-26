# case 02 Smart Fan

![](./images/abtHWmp.jpg)
## Goal



 Make a smart temperature control fan. 

## Materials

 1 x [ELECFREAKS micro:bit Smart Home Kit](https://www.elecfreaks.com/micro-bit-smart-home-kit.html)
 1 x corrugated board
 2 x small sticks
 1 x glue

## Background
  
### Meaning of smart temperature control fan

 The smart temperature control fan is a created product base on smart home.That's say, science come from life.

### What is smart temperature control fan
 The room will at high temperature when temperature degree is higher than 30° and make people feel uncomfortable.The temperature sensor will send this signal to micro:bit，and micro:bit send this signal to the fan. Then, the fan will drive until the degree of room under 30° to keeping room at comfortable temperature.

![](./images/06g0wlF.png)

## Practical operation

Materials: corrugated board and cutter

![](./images/PuJE7uj.jpg)

Build as below picture：

![](./images/5sc9bid.jpg)

Side

![](./images/hvnmUhO.jpg)

Paste devices as below piture:

![](./images/C1lu2Vz.jpg)

## Hardware connect


![](./images/hkOaYEu.png)

## Software

[makecode](https://makecode.microbit.org/#)

Edge Connector Data Sheet

## Programming

### Step 1

Go to MakeCode page, click Advanced in the code block and click on Extensions.

![](./images/2qCyzQ7.png)

We need to add a new codebase for programming of smart home. Finding “Add Package” in the bottom of code block and click it. Then a message box will show up, search “smart home"， and download this new codebase.

![](./images/QR2s7LD.png)

***Note:*** If there is a hint says some codebase will be deleted because of incompatibility. Don't worry. You could go ahead as the hint or build a new item in item menu bar.

### Step 2
Drag on start block from Basic and drag initialize OLED block from OLED, change height to 64, width to 128.

![](./images/NSOCUxe.png)

Drag forever block from Basic, add temp variables in Variable, then drag set item to snap into forever, change item to temp and drag value of temperature behind it. Change value of temperature to ℃ and at pin to P1. 

![](./images/wPfZA5F.png)

### Step 3

Now let's start OLED code.

Drag clear OLED display under set temp to. Then,drag show (without newline) string ‘Temperature’ under clear OLED display. Last, drag show(without newline) number temp."Without newline" is for newline displaying string and temperature value.

![](./images/gZwzVGd.png)

### Step 4

Our goal is using micro:bit driving the fan when the value of temperature is higher than 30°, so temp>30 is a judgement condition. In that way, we need drag "if else" from Logic, set temp>30. 

![](./images/Ys6Hcm3.png)

### Step 5

We add start melody repeating under if ,set melody to ba ding and repeat once，micro:bit will send signal to fan through P2. Then set fan works 5 seconds and stops 5 seconds. The temperature sensor judge whether go loop by gotting the temperature degree. Else means if above condistion were false, the fan will keep rest. 

![](./images/FHAWwTm.png)

### Programming


Make code：[https://makecode.microbit.org/_PKXir0c1V6TX](https://makecode.microbit.org/_PKXir0c1V6TX)

You also could directly download program visit website as below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_PKXir0c1V6TX" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

## Result

When temperature degree is higher than 30°, buzzer "ba ding" , fan driving to keep room comfortable.

![](./images/mv5oVws.jpg)

When temperature degree is less than 30°，the fan will automatically stop, and the room at comfortable temperature.

![](./images/Rtptdzw.jpg)

## Think

How to adjust speed of fan to control cooling rate in the room. 


## Questions

 It works well if powering by the USB only without the battery holders, but if the current temperature is over the threshold value, the fan doesn’t.
 If powering by the battery holders only without the USB, the fan works well and the detected temperature will be slightly higher than the real one.
 If powering by the battery holders and the USB simultaneously, the fan works well and it gets the normal temperature( Do note that you have to detect the temperature under the premise of the motor fan doesn’t drive).
 Please check if you are using micro:bit V2, if yes, please try using the micro:bit V1 instead. If you only have micro:bit V2 , then the sensor:bit with the lastest version should be applied, and you have to power it with the USB port. 
The voltage regulator chip is able to give the current at 1A. Theoretically speaking, the fan can rotate normally. If it cannot rotate, please check whether the USB input current is sufficient. Generally, the computer USB provides 500Ma of current which is able to drive the motor. If the external input current is sufficient and the fan still cannot rotate, please check whether the micro:bit or sensor:bit is damaged.


## More information   

