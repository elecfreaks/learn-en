# case 05 Plant Monitoring Device 

![](./images/kUZLoEo.jpg)

In this article,we are going to talk about how to use micro:bit with buzzer, OLED and moisture sensor to build a case of plant detection device.


## Goals:  
---

- Get to know the buzzer, OLED and moisture sensor.
- Make something with a moisture sensor.

## Products Link

[Tinker Kit](https://www.elecfreaks.com/micro-bit-tinker-kit.html)

## Material Needed:  
---

- 1 x BBC Micro:bit
- 1 x Micro USB Cable
- 1 x Breakout Board
- 1 x Mini Buzzer
- 1 x OLED
- 1 x Moisture Sensor
- 2 x Female-Female Jumper Wires

Note: You can plug components in any sequence.

In this project, we are going to create a plant monitoring which the buzzer will sound when there is not enough water.

A message will always be displaying on the OLED, showing the moisture level.

Firstly, plug in the OLED.
You are able to plug it into any of the three rows.

![](./images/qOBV7Uf.png)

Connect buzzer to P0. Make sure the color of wire follows the pin color on breakout board.

![](./images/ABoiMrD.jpg)

Plug in the moisture sensor to P1.

![](./images/jgTG7i6.jpg)

Click on Advanced in the Code Drawer to see more code sections.
We’ll add a package of code to be able to use our kit components.
Look at the bottom of the Code Drawer for “Add Package” and click it.

![](./images/FOHSrAx.png)

At this time, a dialogue box appears. Search "tinker kit" in the box and then click on the "tinkercademy-tinker-kit" for downloading this package.

![](./images/G2nV10d.png)

Click on Tinkercademy inside the Code Drawer to find our custom blocks for the various components in your kit.

![](./images/57H4sCe.png)
![](./images/DaZC53n.png)

After that, use blocks under the Tinkercademy section to initialize the OLED.

![](./images/xAM8RDr.png)

Since there are only two conditions, we need only one “else-if” statement.
Micro:bit reads values from moisture sensor continuously. 
When the moisture sensor value is less than 50, this indicates that there is not enough water in the pot. As a result, the buzzer will sound and a message “Water your plant” will be displayed on OLED. Else if the moisture sensor value is larger than 50, the buzzer will be in silence and a message “Your plant is in good condition” will be displayed on OLED.

![](./images/qy2wheV.png)

If you don't want to type these code by yourself, you can download the whole program in the link below:
[https://makecode.microbit.org/_DV547gK8j9ms](https://makecode.microbit.org/_DV547gK8j9ms)

Or you can download from this page:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_DV547gK8j9ms" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>


Finally! You have created a device to monitor your plant! Now, let’s try it!

![](./images/nD0PGDe.png)

Download these code into micro:bit. Find a green plant and plug moisture sensor panel into the soil and watch. When there is not enough water, the buzzer will alarm to tell you "it's time to water your plant!". And when the plant has enough water, then the OLED panel will show you water is enough and no need to water the plant.
Isn't it very interesting?

