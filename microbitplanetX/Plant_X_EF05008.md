# Crash Sensor

## Introduction
Crash Sensor is a sensor module based on crash components.

![](./images/05008_01.png)

## Characteristic
---
- Designed in RJ11 connections, easy to plug.
## Specification
---

Item | Parameter 
:-: | :-: 
SKU|EF05008
Connection|RJ11
Type of Connection|Digital output
Working Voltage|3.3V






## Outlook
---


![](./images/05008_02.png)

## Quick to Start

---

### Materials Required and Diagram

---

- Connect the Crash sensor to J1 port and the LED to J2 port in the Nezha expansion board as the picture shows. 


![](./images/05008_03.png)

## MakeCode Programming

---

### Step 1

Click "Advanced" in the MakeCode drawer to see more choices. 

![](./images/05001_04.png)

We need to add a package for programming, . Click "Extensions" in the bottom of the drawer and search with "PlanetX" in the dialogue box to download it. 

![](./images/05001_05.png)

Note: If you met a tip indicating that the codebase will be deleted due to incompatibility, you may continue as the tips say or build a new project in the menu. 

### Step 2

### Code as below:

![](./images/05008_06.png)


### Link
Link: [https://makecode.microbit.org/_Wj9bvpfFm4YK](https://makecode.microbit.org/_Wj9bvpfFm4YK)

You may also download it directly below: 

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Wj9bvpfFm4YK" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  
---

### Result
- The LED lights on if the crash switch was pressed or it lights off. 

## Python Programming 

---


### Step 1

Download the package and unzip it: [PlanetX_MicroPython](https://github.com/lionyhw/PlanetX_MicroPython/archive/master.zip)

Go to   [Python editor](https://python.microbit.org/v/2.0)

![](./images/05001_07.png)

We need to add enum.py and crash.py for programming. Click "Load/Save" and then click "Show Files (1)" to see more choices, click "Add file" to add enum.py and crash.py from the unzipped package of PlanetX_MicroPython. 

![](./images/05001_08.png)
![](./images/05001_09.png)
![](./images/05008_10.png)

### Step 2

### Reference

```
from microbit import *
from enum import *
from crash import *
crash = CRASH(J1)

while True:
    button = crash.crash_is_pressed()
    if(button == True):
        display.show(Image.HAPPY)
    else:
        display.show(Image.SAD)
```


### Result
- A smile face displays on the micro:bit while the crash switch being pressed or the micro:bit displays a sad face.
## Relevant File

---

## Technique File

---
