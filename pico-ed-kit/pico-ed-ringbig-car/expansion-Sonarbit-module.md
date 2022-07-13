# Expansion-Sonar:bit

## Introduction
---
Sonar:bit is a 3-wire ultrasonic module with the working voltage between 3-5V. It is available to be used to 3.3V or 5V micro-controller system. With only one 3-wire(GVS) cable, it can work properly. Compared to the normal 4-wire ultrasonic module, it has saved one IO port. 

The measurement range of sonar:bit is 4cm-400cm. It can output stable and accurate measurement data with ±1cm tolerance only.

It can connect to the [Ring:bit](https://www.elecfreaks.com/elecfreaks-micro-bit-ring-bit-v2-car-kit-without-micro-bit-board.html) with an expansion board.

## Features

Input voltage:3V~5V and can be driven by micro:bit directly.

Standard 3-wire GVS connecotr, which occupies 1 IO port only.

## Parameter

| Item | Parameter | Note |
| --- | --- | --- |
| Name | [Ring:bit](https://www.elecfreaks.com/elecfreaks-micro-bit-ring-bit-v2-car-kit-without-micro-bit-board.html) Car v2  Sonar:bit |  |
| SKU | EF04089 |  |
| Working Voltage | DC 3-5V |  |
| Connections | 3pin GVS Connection ||
||||
| Output signal | Analog |  |
| Measurement | 4~400cm |  |
| Size | 40.60×51.60mm |  |
| NW | 12g |  |

## Outlook and Dimensions
---
## Quick to Start

### Hardware Connections

Connect the acrylic transition board to the back board with the rivets.


Connect the Sonar:bit to the other side of the acrylic transition board with rivets.


Connect the Sonar:bit to the [Ring:bit](https://www.elecfreaks.com/elecfreaks-micro-bit-ring-bit-v2-car-kit-without-micro-bit-board.html) breakout board with a 3-pin wire.

## Programming

Preparation for Programming: [Info](https://www.yuque.com/elecfreaks-learn/picoed/gxro38)

### Samples Code

```python
# Import modules that we need
import board
from ringbit import *

# Set the pins of both wheels
ringbit = Ringbit(board.P1, board.P2)

# Change the speed in accordance with the distances detected by the sonar:bit
while True:
    if ringbit.get_distance(board.P0, Unit.cm) > 20:
        ringbit.set_speed(100, 100)
    else:
        ringbit.set_speed(0, 0)

```
### Details of the program

1. Import the modules that we need. `board` is the common container, and you can connect the pins you'd like to use through it; `ringbit` module contains classes and functions for [Ring:bit](https://www.elecfreaks.com/elecfreaks-micro-bit-ring-bit-v2-car-kit-without-micro-bit-board.html) smart car operations.
```python
import board
from ringbit import *
```

2. Set the pins of the servos
```python
ringbit = Ringbit(board.P1, board.P2)
```

3. While true, set the speed to be controlled by the distance value given by the sonar:bit
```python
while True:
    if ringbit.get_distance(board.P0, Unit.cm) > 20:
        ringbit.set_speed(100, 100)
    else:
        ringbit.set_speed(0, 0)
```
## Result

## Exploration

## FAQ

## Relevant Files
