# Relay Module(EF05025)

## Introduction

It adopts a mini and high-quality HUIKE relay.

![](./images/05025_01.png)


## Products Link

[ELECFREAKS PlanetX PIR Sensor](https://www.elecfreaks.com/planetx-pir.html)

## Characteristic


 Designed in RJ11 connections, easy to plug.

## Specification


Item | Parameter 
:-: | :-:  
SKU|EF05025
Connection|RJ11
Type of Connection|Digital input
Working Voltage|3.3V

## Outlook


![](./images/05025_02.png)

## Quick to Start


### Materials Required and Diagram

 Connect the Relay to J1 port in the Nezha expansion board as the picture shows.


![](./images/05025_03.png)

## MakeCode Programming


### Step 1

Click "Advanced" in the MakeCode drawer to see more choices.

![](./images/05001_04.png)

We need to add a package for programming, . Click "Extensions" in the bottom of the drawer and search with "PlanetX" in the dialogue box to download it. 

![](./images/05001_05.png)

***Note:*** If you met a tip indicating that the codebase will be deleted due to incompatibility, you may continue as the tips say or build a new project in the menu. 

### Step 2

### Code as below:

![](./images/05025_06.png)


### Link
Link: [https://makecode.microbit.org/_FPhJC7K5UYuX](https://makecode.microbit.org/_FPhJC7K5UYuX)

You may also download it directly below: 

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_FPhJC7K5UYuX" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Result
 It switches the current channels by pressing button A or B. 

## Python Programming 


### Step 1

Download the package and unzip it: [PlanetX_MicroPython](https://github.com/lionyhw/PlanetX_MicroPython/archive/master.zip)

Go to  [Python editor](https://python.microbit.org/v/2.0)

![](./images/05001_07.png)

We need to add enum.py and relay.py for programming. Click "Load/Save" and then click "Show Files (1)" to see more choices, click "Add file" to add enum.py and relay.py from the unzipped package of PlanetX_MicroPython. 

![](./images/05001_08.png)
![](./images/05001_09.png)
![](./images/05025_10.png)

### Step 2

### Reference

```
from microbit import *
from enum import *
from relay import *

l = RELAY(J1)
l.set_relay(1)
```


### Result
 Control the off/on of the Relay. 

## Relevant File


## Technique File

