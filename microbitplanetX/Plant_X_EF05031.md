# MQ2 Gas Sensor(EF05031)

## Introduction

MQ2 Gas sensor is used in gas leakage detecting equipments in consumer and industry markets, this sensor is suitable for detecting LPG, i-butane, propane, methane ,alcohol, hydrogen and smoke. 

![](./images/05031_01.png)
## Products Link

[ELECFREAKS PlanetX MQ2 Sensor](https://www.elecfreaks.com/planetx-mq2.html)

## Characteristic


 Designed in RJ11 connections, easy to plug.

## Specification


Item | Parameter 
:-: | :-: 
SKU|EF05031
Connection|RJ11
Type of Connection|Analog output
Working Voltage|3.3V


## Outlook



![](./images/05031_02.png)

## Quick to Start


### Materials Required and Diagram

 Connect the MQ2 Gas sensor to J1 port and the OLED to the IIC port in the Nezha expansion board as the picture shows.


![](./images/05031_03.png)

***Note:*** A preheating for 3 minutes after powering on is required before using.

## MakeCode Programming


### Step 1

Click "Advanced" in the MakeCode drawer to see more choices.

![](./images/05001_04.png)

We need to add a package for programming, . Click "Extensions" in the bottom of the drawer and search with "PlanetX" in the dialogue box to download it. 

![](./images/05001_05.png)

***Note:*** If you met a tip indicating that the codebase will be deleted due to incompatibility, you may continue as the tips say or build a new project in the menu. 

### Step 2

### Code as below:

![](./images/05031_06.png)


### Link
Link: [https://makecode.microbit.org/_DeX9DA369Amq](https://makecode.microbit.org/_DeX9DA369Amq)

You may also download it directly below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_DeX9DA369Amq" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Result
 The value detected from MQ2 Gas sensor displays on the OLED screen.

## Python Programming 


### Step 1

Download the package and unzip it: [PlanetX_MicroPython](https://github.com/lionyhw/PlanetX_MicroPython/archive/master.zip)

Go to  [Python editor](https://python.microbit.org/v/2.0)

![](./images/05001_07.png)

We need to add enum.py and smoke.py for programming. Click "Load/Save" and then click "Show Files (1)" to see more choices, click "Add file" to add enum.py and smoke.py from the unzipped package of PlanetX_MicroPython. 

![](./images/05001_08.png)
![](./images/05001_09.png)
![](./images/05031_10.png)

### Step 2

### Reference

```
from microbit import *
from enum import *
from smoke import *
smoke = SMOKE(J1)
while True:
    display.scroll(smoke.get_smoke())
```


### Result
 The value detected from MQ2 Gas sensor displays on the micro:bit.

## Relevant File


## Technique File

