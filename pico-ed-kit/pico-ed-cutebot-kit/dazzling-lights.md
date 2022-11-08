# Case 05: Dazzling Lights

## Introduction
Make [Cutebot](https://shop.elecfreaks.com/products/elecfreaks-pico-ed-smart-cutebot-kit-with-pico-ed-board?_pos=2&_sid=40bbc85e4&_ss=r) drive forward and display random light colors.
## Programming Preparation
Please refer to: [Preparing the Programming Environment](http://www.elecfreaks.com/learn-en/pico-ed-kit/pico-ed-cutebot-kit/preparation-for-the-programming.html)
## Sample code
```python
from cutebot import *
from random import *
from time import *

# Create a sample for Cutebot category
cutebot = Cutebot()    

#  Set the cutebot smart car to drive forward at 50% speed
cutebot.set_speed(50,50)
# Initialize the rainbow light
cutebot.init_rainbow_leds()

#  While true, change the color of the headlights and the Rainbow LED at random. 
while True:
while True:
    R = randint(0, 255)
    G = randint(0, 255)
    B = randint(0, 255)
    cutebot.set_light(RGB.left,R,G,B)
    cutebot.set_light(RGB.right,R,G,B)
    cutebot.rainbow_leds[0] = (R,G,B)
    cutebot.rainbow_leds[1] = (R,G,B)
    sleep(1)
```
###  Code details

1. Import the modules that we need for the program: `cutebot` module contains classes and functions that operate on Cutebot smart cars, `time` module contains functions that operate on time, `random` module contains functions that generate random numbers.
```python
from cutebot import *
from random import *
from time import *
```

2. Create a sample for Cutebot category
```python
cutebot = Cutebot()
```

3. Set the cutebot smart car to drive forward at 50% speed and initialize the rainbow lights.
```python
cutebot.set_speed(50,50)
cutebot.init_rainbow_leds()
```

4. While true, change the color of the headlights and the Rainbow LED at random.
```python
while True:
    R = randint(0, 255)
    G = randint(0, 255)
    B = randint(0, 255)
    cutebot.set_light(RGB.left,R,G,B)
    cutebot.set_light(RGB.right,R,G,B)
    cutebot.rainbow_leds[0] = (R,G,B)
    cutebot.rainbow_leds[1] = (R,G,B)
    sleep(1)
```
## Results
After powering on, the cutebot smart car moves forward and the lights change the colours at random. 
## Exploration
How do you make the lights switch colors automatically according to the speed of the cutebot smart car?
