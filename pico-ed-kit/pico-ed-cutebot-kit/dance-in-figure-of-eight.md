# Case 03: Dance in Figure-of-eight

## Introduction
Make [Cutebot](https://shop.elecfreaks.com/products/elecfreaks-pico-ed-smart-cutebot-kit-with-pico-ed-board?_pos=2&_sid=40bbc85e4&_ss=r) travel along a figure-of-8 track.
## Programming Preparation
Please refer to: [Preparation for the Programming](http://www.elecfreaks.com/learn-en/pico-ed-kit/pico-ed-cutebot-kit/preparation-for-the-programming.html)
##  Sample code :
```python
from cutebot import *
from time import *

# Create a sample for Cutebot category
cutebot = Cutebot()

# Turnning by adjusting the different speed of the left and right wheels of the cutebot. 
while True:
    cutebot.set_speed(100,50)
    sleep(2)
    cutebot.set_speed(50,100)
    sleep(2)
```
### Code details

1. Import the modules that we need: `cutebot `module contains classes and functions for Cutebot smart car operations, and `time ` module contains functions for time operations.
```python
from cutebot import *
from time import *
```

2.  Create a sample for Cutebot category
```python
cutebot = Cutebot()
```

3. Directions turning is done by controlling the speed difference between the left and right wheels of the cutebot smart car.
```python
while True:
    cutebot.set_speed(100,50)
    sleep(2)
    cutebot.set_speed(50,100)
    sleep(2)
```
## Results
After turning on the power, the cutebot smart car travels in a figure of 8 trajectory.
## Exploration
How should I program the car if I want it to travel in a square trajectory?
