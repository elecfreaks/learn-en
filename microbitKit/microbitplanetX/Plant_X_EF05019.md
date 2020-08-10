# Two Channels Tracking Module

## Introduction
The two channels Tracking Module has integrated two groups of reflective infrared pair diode, which can be used to make line tracking smart cars. 

![](./images/05019_01.png)

## Characteristic

---

- Designed in RJ11 connections, easy to plug.

## Specification

---

Item | Parameter 
:-: | :-: 
SKU|EF05019
Connection|RJ11
Type of Connection|Digital output
Working Voltage|3.3V
Effective Distance|2~12mm
Black Line|Low level output
White Line|High level output





## Outlook
---


![](./images/05019_02.png)

## Quick to Start

---

### Materials Required and Diagram

---

- Connect the Two channels tracking module to J1 port in the Nezha expansion board as the picture shows.


![](./images/05019_03.png)

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

![](./images/05019_06.png)


### Link
Link: [https://makecode.microbit.org/_hy3VDtA3xAqE](https://makecode.microbit.org/_hy3VDtA3xAqE)

You may also download it directly below: 

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_hy3VDtA3xAqE" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  
---

### Result
- Different icons display on the micro:bit in accordance with the different status detected by the tracking module.

## Python Programming 

---

### Step 1

Download the package and unzip it: [PlanetX_MicroPython](https://github.com/lionyhw/PlanetX_MicroPython/archive/master.zip)

Go to  [Python editor](https://python.microbit.org/v/2.0)

![](./images/05001_07.png)

We need to add enum.py and tracking.py for programming. Click "Load/Save" and then click "Show Files (1)" to see more choices, click "Add file" to add enum.py and tracking.py from the unzipped package of PlanetX_MicroPython. 

![](./images/05001_08.png)
![](./images/05001_09.png)
![](./images/05019_10.png)

### Step 2

### Reference

```
from microbit import *
from enum import *
from tracking import *

tracking = TRACKING(J1)
while True:
    if tracking.get_state() == 11:
        display.show(Image.YES)
    elif tracking.get_state() == 10:
        display.show(Image.SAD)
    elif tracking.get_state() == 00:
        display.show(Image.NO)
    elif tracking.get_state() == 01:
        display.show(Image.HAPPY)
```


### Result
- Different icons display on the micro:bit in accordance with the different status detected by the tracking module.
## Relevant File

---

## Technique File

---
