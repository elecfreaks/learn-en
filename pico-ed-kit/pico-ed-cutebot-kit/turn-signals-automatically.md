# Case 04: Turn Signals Automatically

## Introduction
Make [Cutebot](https://shop.elecfreaks.com/products/elecfreaks-pico-ed-smart-cutebot-kit-with-pico-ed-board?_pos=2&_sid=40bbc85e4&_ss=r) follow a random route and turn on the turn signal automatically.

## Programming Preparation
Please refer to: [Preparing Programming Environment](http://www.elecfreaks.com/learn-en/pico-ed-kit/pico-ed-cutebot-kit/preparation-for-the-programming.html)
## Sample code
```python
from cutebot import *
from random import *
from time import *

# Create a sample for Cutebot category
cutebot = Cutebot()

# Assign the random value among (0,100) to the speed for the two wheels, turn on the sigals light automatically in accordance with the driving directions of the Cutebot. 
while True:
    left_speed = randint(0, 100)
    right_speed = randint(0, 100)
    if left_speed > right_speed:
        cutebot.set_light(RGB.left,0,0,0)
        cutebot.set_light(RGB.right,255,255,0)
    if left_speed < right_speed:
        cutebot.set_light(RGB.left,255,255,0)
        cutebot.set_light(RGB.right,0,0,0)
    cutebot.set_speed(left_speed,right_speed)
    sleep(2)
```
###  Code details

1. Import the modules that we need for the program：`cutebot` module contains the classes and functions that operate on Cutebot smart cars, `time` module contains the functions that operate on time, `random` module contains the functions that generate random numbers.
```python
from cutebot import *
from random import *
from time import *
```

2. Create a sample for Cutebot category
```python
cutebot = Cutebot()
```

3. Assign the random value among (0,100) to the speed for the two wheels, turn on the sigals light automatically in accordance with the driving directions of the Cutebot. 
```python
while True:
    left_speed = randint(0, 100)
    right_speed = randint(0, 100)
    if left_speed > right_speed:
        cutebot.set_light(RGB.left,0,0,0)
        cutebot.set_light(RGB.right,255,255,0)
        if left_speed < right_speed:
            cutebot.set_light(RGB.left,255,255,0)
            cutebot.set_light(RGB.right,0,0,0)
            cutebot.set_speed(left_speed,right_speed)
    sleep(2)
```
## Results
After turning on the power, the cutebot smart car travels on a random trajectory and automatically lights up the turn signal according to the direction the smart car is traveling.
## Exploration
When the speed of the left and right wheels of the car is the same, how can we program the two headlights of the cutebot smart car to light up at the same time?
