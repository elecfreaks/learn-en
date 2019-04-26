# sonar:bit 

## Introduction
---

Sonar:bit is an ultrasonic module with 3-5V working voltage. It is available to be used to 3.3V or 5V micro-controller system. With only one 3-wire(GVS) cable, it can work properly. Compared to the normal 4-wire ultrasonic module, it has saved one IO port. The measurement range of sonar:bit is 4cm-400cm. It can output stable and accurate measurement data with ±1cm tolerance only. You can use this module to occasions like short-distance measurement, smart cars, robots, micro:bit and arduino teaching, etc..

![](./images/pdBREKf.jpg)


## Features
---
- Input voltage:3V~5V
- Enable to drive micro:bit or arduino directly.
- Standard 3-wire GVS connecotr, which occupies 1 IO port only. 

## Parameter
---

![](./images/G7YHeuJ.png)


## Dimension
---
![](./images/h4HcvxO.jpg)

## Definition of Pins
---
![](./images/7E5ECzN.jpg)


## Introduction of Major Components
---

### Transmitter

![](./images/T1xDsne.jpg)

Transmitter is used to send ultrasonic signals. 

### Receiver

![](./images/JxNrz8Q.jpg)

Receiver is for collecting ultrasonic signals. 

### MCU

![](./images/2CjnvfP.jpg)

This is the master chip of sonar:bit. 

### Chip for Sending Signal

![](./images/iOW0IN3.jpg)

This chip is used to drive the transmitter to send out ultrasonic signals. 

### Chip for Receiving Signal

![](./images/VxEZ5KQ.jpg)

This chip is used to receive and process ultrasonic echo signals as well as give feedbacks to the master chip. 

### G-V-S Port

![](./images/N9yc6Jm.jpg)

G-V-S port allows outer devices control.


## Quick Start
---

### Hardware Connection  

Connect sonar:bit to P2 port on sensor:bit and connect micro:bit to your computer.  
Once completed, you can see the picture below:

![](./images/fvYx5lR.jpg)

![](./images/wCftg3Y.jpg)

### Programming

Click to open [Makecode](https://makecode.microbit.org/) online editor.

Write your program to assign the returned value of P2 to variable distance and display it on micro:bit screen.

![](./images/sbRh3HL.png)

You can see the whole program from the link here: [https://makecode.microbit.org/_b7JL2Yd3q3Km](https://makecode.microbit.org/_b7JL2Yd3q3Km)

Or you can download it from the page below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_b7JL2Yd3q3Km" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### Result

We can see the distance between sonar:bit and the object is displayed on micro:bit in real time. The unit is centimeter. 


## Document
---
WIKI


## FAQ
---
