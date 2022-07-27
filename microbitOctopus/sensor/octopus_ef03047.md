# Color Sensor Module(EF03047)

## Introduction


Based on TCS3200, the Color sensor module is a programmable color light-to-frequency converter, it could filter RGB data from source light and convert it to a square wave(50% duty cycle) with frequency directly proportional to light intensity (irradiance). The full-scale output frequency can be scaled by one of three preset values via two control input pins(SO, S1 Selectable Options 2%, 20%, 100% frequency),and pin S2, S3 control the filter of RGB. Digital input and output allow interface to a microcontroller or other logic circuitry directly. Output enable (OE) places the output in the high-impedance state for multiple-unit sharing of a microcontroller input line. At last, user can calculate the color of the light by RGB values. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitOctopus/sensor/images/03047_00.jpg)

## Characteristics

 High-resolution conversion of light intensity to frequency
 Programmable color and full-scale output frequency
 Communicating directly with a microcontroller
 Single-supply operation (2.7 V to 5.5 V)
 Nonlinearity error typically 0.2% at 50 kHz
 Stable 200 ppm/°C temperature coefficient

## Parameter

 Name: Color Sensor Module
 SKU：EF03047
 Working Voltage: DC 2.7~5.5V
 Connection Mode: G-GND，V-VCC，S-signal pins
 Size: 37.6 x 37.6mm
 Net Weight: 5.1g

## Outlook and Dimmensions


![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitOctopus/sensor/images/03047_01.png)

## Quick to Start

### Hardware Connection

Connect S0 to pin15,  S1 to P1,  S2 to P8,  S3 to P12,  OUT to P2,  VCC to the Power Supply and GND to the GND.  Then insert the micro:bit to Octopus:bit.
Connect OLED to IIC port.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitOctopus/sensor/images/03047_02.png)

### Software Programming

Add extension library:[https://github.com/DoraLC/pxt-tcs3200-color-sensor](https://github.com/DoraLC/pxt-tcs3200-color-sensor)

Show RGB value to OLED.

Links: [https://makecode.microbit.org/_JU5Dau19mE9c](https://makecode.microbit.org/_JU5Dau19mE9c)

You can also download it directly below:
<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_JU5Dau19mE9c" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### Result

The value of the current red, blue and green is displaying on the OLED screen.

## FAQ

Avoid the interference of outside light,testing the better in a confined space
No special requirements for light, but try to focus on a single
The first use or restart or change light and so on, please adjust the WB(White Balance)
