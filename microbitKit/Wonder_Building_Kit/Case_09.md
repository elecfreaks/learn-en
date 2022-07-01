# Case 09: Automatic Doors

## Purpose
---
To make an automatic door. 
 
![](./images/case-09-01.png)

## Link: 
---
[micro:bit Wonder Building Kit](https://www.elecfreaks.com/micro-bit-wonder-building-kit-without-micro-bit-board.html)

## Materials Required
---
![](./images/case-09-02.png)

Video link:
[https://youtu.be/JimDF7ArSjQ](https://youtu.be/JimDF7ArSjQ)


## Bricks build-up
---


![](./images/step-case-09-01.png)

![](./images/step-case-09-02.png)

![](./images/step-case-09-03.png)

![](./images/step-case-09-04.png)

![](./images/step-case-09-05.png)

![](./images/step-case-09-06.png)

![](./images/step-case-09-07.png)

![](./images/step-case-09-08.png)

![](./images/step-case-09-09.png)

![](./images/step-case-09-10.png)

![](./images/step-case-09-11.png)

![](./images/step-case-09-12.png)

![](./images/step-case-09-13.png)

![](./images/step-case-09-14.png)

![](./images/step-case-09-15.png)

![](./images/step-case-09-16.png)

![](./images/step-case-09-17.png)

![](./images/step-case-09-18.png)

![](./images/step-case-09-19.png)

![](./images/step-case-09-20.png)

![](./images/step-case-09-21.png)

![](./images/step-case-09-22.png)

## Installation Mthods of Hardwares

Install the sonar:bit with the bricks. 

![](./images/Wonder-Building-Kit-step-sonar-bit-3.png)

## Hardware Connection

Connect a [sonar:bit](https://www.elecfreaks.com/sonar-bit-for-micro-bit-ultrasonic-sensor-distance-measuring-3v-5v.html) to P1 and the [servo](https://www.elecfreaks.com/geekservo-2kg-360-degrees-compatible-with-lego.html) to S0 port on [Wukong breakout board](https://www.elecfreaks.com/wukong-board-with-lego-holder-for-micro-bit.html). 

![](./images/Wonder-Building-Kit-case-09-06.png)

## Software Platform
---
[MakeCode](https://makecode.microbit.org/)

## Coding
---
### Add extensions
Click "Advanced" in the MakeCode to see more choices.
 
![](./images/case-01-03.png)

Search with Wukong in the dialogue box to download it. 

![](./images/case-01-04.png)

 Search with https://github.com/elecfreaks/pxt-sonarbit in the dialogue box to add the sonar:bit extension. 

![](./images/case-04-04.png)



### Program
 
![](./images/case-09-03.png)

Link:[https://makecode.microbit.org/_eUPf4XEudVKY](https://makecode.microbit.org/_eUPf4XEudVKY)

### Result

When the ultrasonic sensor detects someone passing by, it will display √ on the micro:bit and control the servo to open the door and close it automatically after 5 seconds, if the ultrasonic sensor does not detect anyone, it will keep displaying × on the micro:bit and the door is closed.
