# RTC Real-time Module(EF05034)

## Introduction
---
It is a clock module which can achieve counting for year, month, day, hour, minute and second by using the DS1307 clock chip.

![](./images/05034_01.png)

## Characteristic
---

- Designed in RJ11 connections, easy to plug.

## Specification
---

Item | Parameter 
:-: | :-: 
SKU|EF05034
Connection|IIC
Type of Connection|Analog output
Working Voltage|3.3V
Core IC|DS1307


## Outlook
---


![](./images/05034_02.png)

## Quick to Start
---

### Materials Required and Diagram

- Connect the RTC Real-time module to the IIC port and the OLED to another IIC port in the Nezha expansion board as the picture shows.


![](./images/05034_03.png)



## MakeCode Programming
---

### Step 1

Click "Advanced" in the MakeCode drawer to see more choices.

![](./images/05001_04.png)

We need to add a package for programming, . Click "Extensions" in the bottom of the drawer and search with "PlanetX" in the dialogue box to download it. 

![](./images/05001_05.png)

***Note:*** If you met a tip indicating that the codebase will be deleted due to incompatibility, you may continue as the tips say or build a new project in the menu. 

### Step 2

### Code as below:

![](./images/05034_06.png)


### Link
Link: [https://makecode.microbit.org/_fEwJ9E1sf8jA](https://makecode.microbit.org/_fEwJ9E1sf8jA)

You may also download it directly below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_fEwJ9E1sf8jA" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Result
- The seconds read by the RTC Real-time module displays on the OLED screen.

## Python Programming 
---

### Step 1

Download the package and unzip it: [PlanetX_MicroPython](https://github.com/lionyhw/PlanetX_MicroPython/archive/master.zip)

Go to  [Python editor](https://python.microbit.org/v/2.0)

![](./images/05001_07.png)

We need to add ds1370.py for programming. Click "Load/Save" and then click "Show Files (1)" to see more choices, click "Add file" to add ds1370.py from the unzipped package of PlanetX_MicroPython. 

![](./images/05001_08.png)
![](./images/05001_09.png)
![](./images/05034_10.png)

### Step 2

### Reference

```
from microbit import *
from ds1307 import *

ds1307 = DS1307()
ds1307.Second(second=0)
while True:
    display.scroll(ds1307.Second())
```


### Result
- The seconds read by the RTC Real-time module displays on the micro:bit.

## Relevant File
---

## Technique File
---
