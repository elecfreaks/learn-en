# Case 08: IR Remote Control Car

## Introduction
Control [Cutebot](https://www.elecfreaks.com/elecfreaks-pico-ed-smart-cutebot-kit-with-pico-ed-board.html)  to drive by remote control.
## Programming Preparation
Please refer to：[Preparing Programming Environment](https://www.yuque.com/elecfreaks-learn/picoed/gccnpl)
##  Infrared remote control key value table

| key | return value | key | return value | key | return value |
| --- | --- | --- | --- | --- | --- |
| Power | 11 |||||
 | 
 | MENU | 12 |
| + | 13 | UP | 14 | Return | 15 |
| Left| 16 | OK | 17 |Right| 18 |
| - | 19 | Down | 20 | 0 | 0 |
| 1 | 1 | 2 | 2 | 3 | 3 |
| 4 | 4 | 5 | 5 | 6 | 6 |
| 7 | 7 | 8 | 8 | 9 | 9 |

## Sample code
```python
from cutebot import *

# Create a sample for Cutebot category
cutebot = Cutebot()    

# While true, keep detecting the values received by the IR receiver
# Control the route of the Cutebot based on the received value
while True:
    Ir = cutebot.get_ir_value()
    if Ir == 14:
        cutebot.set_speed(50, 50)
    if Ir == 16:
        cutebot.set_speed(-30, 30)
    if Ir == 17:
        cutebot.set_speed(0, 0)
    if Ir == 18:
        cutebot.set_speed(30, -30)
    if Ir == 20:
        cutebot.set_speed(-50, -50)
```
###  Code details

1. Import the modules that we need for the program: `cutebot ` module contains the classes and functions that operate on the Cutebot smart car.
```python
from cutebot import *
```

2. Create a sample for Cutebot category.
```python
cutebot = Cutebot()
```

3. While true, keep detecting the values received by the IR receiver.Control the route of the Cutebot based on the received value.
```python
while True:
    Ir = cutebot.get_ir_value()
    if Ir == 14:
        cutebot.set_speed(50, 50)
    if Ir == 16:
        cutebot.set_speed(-30, 30)
    if Ir == 17:
        cutebot.set_speed(0, 0)
    if Ir == 18:
        cutebot.set_speed(30, -30)
    if Ir == 20:
        cutebot.set_speed(-50, -50)
```
## Results
After turning on the power, the Cutebot is controlled by IR remote control to drive.
## Exploration
Is it possible to control more functions of the Cutebot by IR remote control?
