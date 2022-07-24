# Case 02: Speed Up Gradually

## Introduction
Control the [Cutebot](https://www.elecfreaks.com/elecfreaks-pico-ed-smart-cutebot-kit-without-pico-ed-board.html) to accelerate evenly until it reaches the maximum speed.
##  Programming Preparation
Please refer to: [Preparing the Programming Environment](https://www.yuque.com/elecfreaks-learn/picoed/gccnpl)
## Sample code
```python
from cutebot import *
from time import *

#  Create a sample for Cutebot category
cutebot = Cutebot()
#  Create the variable cutebot_speed to hold the speed value of the cutebot smart car
cutebot_speed = 0

# Set the speed of the cutebot smart car to accelerate evenly from 0 to 100
while True:
    if cutebot_speed > 100:
        cutebot_speed = 100
    cutebot.set_speed(cutebot_speed,cutebot_speed)
    cutebot_speed = cutebot_speed + 1
    sleep(0.02)
```
### Code details

1.  Import the modules that we need:  `cutebot`module contains the classes and functions for Cutebot smart car operation, `time `module contains the functions for time operation.
```python
from cutebot import *
from time import *
```

2.  Create a sample for Cutebot category
```python
cutebot = Cutebot()
```

3.  Create the variable cutebot_speed to hold the speed value of the cutebot.
```python
cutebot_speed = 0
```

4.  Set the speed of the cutebot to accelerate evenly from 0 to 100.
```python
while True:
    if cutebot_speed > 100:
        cutebot_speed = 100
        cutebot.set_speed(cutebot_speed,cutebot_speed)
        cutebot_speed = cutebot_speed + 1
    sleep(0.02)
```
## Results
After turning on the power, the speed of cutebot accelerates evenly from 0~100.
## Exploration
How to make the car accelerate evenly and then decelerate evenly?
