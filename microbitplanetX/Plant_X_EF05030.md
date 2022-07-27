# CO2 Gas Sensor(EF05030)

## Introduction

The higher the CO2 concentration is, the lower the output voltage would be. The CO2 probe is made with industrial grade which is high allergic to CO2 and anti-interference to alcohol and CO. 

![](./images/05030_01.png)
## Products Link

[ELECFREAKS PlanetX CO2 Sensor](https://www.elecfreaks.com/planetx-co2.html)

## Characteristic


 Designed in RJ11 connections, easy to plug.

## Specification


Item | Parameter 
:-: | :-: 
SKU|EF05030
Connection|RJ11
Type of Connection|Analog output
Working Voltage|3.3V

## Outlook



![](./images/05030_02.png)

## Quick to Start


### Materials Required and Diagram

 Connect the CO2 sensor to J1 port and the OLED to the IIC port in the Nezha expansion board as the picture shows.


![](./images/05030_03.png)


## MakeCode Programming


### Step 1

Click "Advanced" in the MakeCode drawer to see more choices.

![](./images/05001_04.png)

We need to add a package for programming, . Click "Extensions" in the bottom of the drawer and search with "PlanetX" in the dialogue box to download it. 

![](./images/05001_05.png)

***Note:*** If you met a tip indicating that the codebase will be deleted due to incompatibility, you may continue as the tips say or build a new project in the menu. 

### Step 2

### Code as below:

![](./images/05030_06.png)


### Link
Link: [https://makecode.microbit.org/_2mT2MxX236EM](https://makecode.microbit.org/_2mT2MxX236EM)

You may also download it directly below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_2mT2MxX236EM" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Result
 The detected value of the CO2 Gas sensor display on the OLED screen.

## Python Programming 


### Step 1

Download the package and unzip it: [PlanetX_MicroPython](https://github.com/lionyhw/PlanetX_MicroPython/archive/master.zip)

Go to  [Python editor](https://python.microbit.org/v/2.0)

![](./images/05001_07.png)

We need to add enum.py and CO2.py for programming. Click "Load/Save" and then click "Show Files (1)" to see more choices, click "Add file" to add enum.py and CO2.py from the unzipped package of PlanetX_MicroPython. 

![](./images/05001_08.png)
![](./images/05001_09.png)
![](./images/05030_10.png)

### Step 2

### Reference

```
from microbit import *
from enum import *
from co2 import *
co2 = CO2(J1)
while True:
    display.scroll(co2.get_co2())
```


### Result
 The detected value of the CO2 Gas sensor display on the micro:bit.

## Relevant File


## Technique File

