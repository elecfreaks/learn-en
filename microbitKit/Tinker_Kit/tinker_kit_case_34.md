# case 34 micropython 

## Getting Started
---


### Pre-coding:
---
- Get hold of a Micro:bit Tinker Kit
- Download the Mu editor
[Mu editor](https://codewith.mu/)

           

## Project 01: Music Machine
---
![](./images/gXqhVI7.jpg)

**Pin Layout**

- Buzzer: Pin0
- ADKeypad: Pin2

**Small note about the ADKeypad**


The ADKeypad returns an analog signal when its buttons are pressed. Each button pressed would return a unique integer value ranging from 0 (meaning 0V) to 1023 (meaning 3V). 
However, it is not uncommon that each button would give a small range of values when pressed at different times and different ADKeypads might give different signals yet again. Hence, in this example code, we provide a range of possible values that your ADKeypad’s buttons are likely to return when pressed. 
Feel free to test out the values that your ADKeypad might return when pressed and change the values in the example code. ^ ^

![](./images/8xVE2p6.png)


## Project 02: Smart Light
---
![](./images/qIQKK4y.jpg)

**Pin Layout**

- PIR Sensor: Pin0
- LED: Pin1
![](./images/7Dgi7Wt.png)

## Project 03: Electro-Theremin
---
![](./images/Njalhk0.jpg)

**Pin Layout**

- Buzzer: Pin0
- Potentiometer: Pin1

![](./images/CBFkYTp.png)


## Project 04: Simple Alarm Box
---
![](./images/gWAmEhW.jpg)

**Pin Layout**

- Crash Sensor: Pin0
- LED: Pin8
- OLED: I2C row (at the bottom of the BoB)


![](./images/R4XO4S6.png)

![](./images/01GlIIR.png)
 
## Project 05: Plant Monitoring Device
---
![](./images/JBmCc6A.jpg)       
 
**Pin Layout**

- Buzzer: Pin0
- Soil Moisture Sensor: Pin1
- OLED: I2C row (at the bottom of the BoB)

![](./images/bOGavUM.png)

![](./images/guZyD53.png)


### Get Creative!
---
Mix and match the component in the Tinker Kit to create your own projects.

For a more comprehensive explanation of MicroPython, visit the official documentation [here](https://microbit-micropython.readthedocs.io/en/latest/tutorials/introduction.html)







