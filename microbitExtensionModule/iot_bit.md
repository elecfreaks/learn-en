# iot:bit(EF03426)

## Introduction
---

- [IoT:bit](https://www.elecfreaks.com/iot-bit-for-micro-bit.html) is an expansion board based on IoT for micro:bit. It uses ESP8266 as WIFI expansion board and serial port to communicate with micro:bit. It also has extended all available IO port of the micro:bit which is leaded by GVS and you can extent various 3V E-blocks as LED, photosensitive and servo by using it. At the same time, the IOT:bit with an on-board buzzer for outside sound and an on-board RTC clock for timing without power supply. Let's creating your own IoT by makecode!

 ![](./images/NGKCsKq.jpg)

### Features


- Intergrated ESP12F WiFi、RTC and passive buzzer module
- Extended most IO ports by GVS
- Silk-screen indication onboard main components
- Separately lead IIC interface, directly plug in OLED, BME280 and IIC,etc
- Intergrated buzzer and earphone jack
- Adaptive for LEGO (4 standard spacing Lego fixed holes)

## Hardware apperance & Parameters 
---

### Size & Installation 


- Product size：71mm x 63mm x 23mm
- PCB thickness：1.5mm
- Hole diameter：2.4mm

 ![](./images/5CDXW5R.png)

### Parameters


 |Items|Parameters|Remarks|
 |:-:|:-:|:-:|
 |DC supply|USB-5V|-|
 |Maximum power current|800mA|-|
 |Operation temperature|-25~80℃|-|
 |WIFI module|ESP8266|ESP12F|
 |Buzzer|Passive buzzer|-|
 |RTC timing|DS1307 RTC|-|
 |RTC timing battery|CR1220 button cell|Equipped by yourself|
 |Lead out|Not all|-|
 |port lead|Serial port can map the IO port|Coding|
 |I2C port lead|19、20 pin|Only for I2C pin|
 |SPI port lead|14、15 pin|for common IO|
 |Size|71.00mm X 63.00mm|Without packing|
 |Net weight|30.00g|Without packing|

### Pin interface drawing


![](./images/3Pb4vCV.png)

### Introduction of main module


 ![](./images/bkO3DMr.png)

## Software support
---

- Coding：Makecode/Micropython/JavaScript/

### Makecode block


- Coding developed by Microsoft and mainly publiced by micro:bit offical.

- https://makecode.microbit.org

 ![](./images/LczawXh.png)

### JavaScript


- Click on `JavaScript` of the `makecode` for `JavaScript` coding.

- https://makecode.microbit.org

 ![](./images/X7zJlwA.png)

### MicroPython 


- Using `MU` for advanced coding method`MicroPython` 

- https://codewith.mu/

 ![](./images/CJytOdT.png)


## Easy start 
---
### Hardware connection

- Fisrt, install CR1220 button cell for power supply to the RTC timing. 

 ![](./images/EkM7aP2.gif)

- Plug the micro:bit to the Iot:bit.

 ![](./images/kFW4hB9.gif)

- Using single USB for power supply to expansion board and switch on.  

 ![](./images/DXB3mBI.gif)

### Coding  

#### Coding Platform ####


- makecode：https://makecode.microbit.org


#### Add codebase ####


- Click on "Advanced" in the MakeCode Drawer to see more code sections.

 ![](./images/j31P9Bx.jpg)

- We need to add an extension for coding to the IOT. Click on the “Extension” at bottom of coding drawer, then Search for “IOT” and click on the IOT package to add it to your project. (As below picture) 

 ![](./images/AaZxCEb.jpg)

***Note：*** If you get a warning telling you some packages will be removed because of incompatibility issues, either follow the prompts or create a new project in the Project file menu.


#### How to drive the buzzer ####


- There is on-board buzzer on the IOT:bit as below picture. Let the buzzer be connected to the PO of the micro:bit to play music by the `music` of the makecode.

 ![](./images/zBNYZsy.png) ![](./images/lNibSJk.png)

- When button A be pressed in the "input", play a bit of music. 

 ![](./images/cPG4w9y.png)

- Program link：[https://makecode.microbit.org/_4j6PCeV087AW](https://makecode.microbit.org/_4j6PCeV087AW)


#### How to use RTC ####


- There is on-board DS1307RTC timing on the IOT:bit as below picture. RTC timing need a CR1220 button cell for lasting power supply. We need the RTC timing keep accuracy in the event of a power outage. 

 ![](./images/Y76pQRh.jpg) ![](./images/ivqmwe3.png)



- Press button A to set the time to the set time. On start with RTC function and the minutes be displayed on the 5*5 allay.

-   Turn off the power after turning off the power for one minute, and the dot matrix display will show the number of minutes after another 1 minute.

 ![](./images/t9fOHMT.png)

- Program link：[https://makecode.microbit.org/_e9d3vW96bPe2](https://makecode.microbit.org/_e9d3vW96bPe2)

#### How to use the internet function ####


- The most important function of IOT:bit is WIKI. The onboard `ESP-12F`WIFI module can connect WIFI and send information. To use port for communication with the micro:bit and the pin `RX-P8`，`TX-P12` is special for IoT.
- Using thingspeak as cloud to coding and data uploding.[thingspeak平台使用指南]()

 ![](./images/CbzmpB1.jpg) ![](./images/fLnI2rl.png)

- On start, initialize ESP8266 to default connection with P8 & P12.
- Connect your own WiFi, input the key and the password.
- Under foever loop, connect the thinkspeak and set date to send, then pause. 

 ![](./images/03PNnhW.png)

- Program link：[https://makecode.microbit.org/_JAXAmmHq4FhW](https://makecode.microbit.org/_JAXAmmHq4FhW)

### Down load code ###

- Let your micro:bit be connected to one side of the USB, the other side to your computer.（Inserting on the expansion board may cause the micro:bit connection to be abnormal or damaged.）

![](./images/DfE3smq.jpg)

- Then copy your documents to the micro:bit. 

- Now, here is your observing time!

![](./images/YEGtIO7.jpg)

### Documents 



### More information

