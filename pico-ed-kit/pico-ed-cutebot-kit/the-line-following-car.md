# Case 06: The Line-following Car

## Introduction
Make [Cutebot ](https://www.elecfreaks.com/elecfreaks-pico-ed-smart-cutebot-kit-without-pico-ed-board.html)drive along the black line.
## Programming Preparation
Please refer to: [Preparing Programming Environment](https://www.yuque.com/elecfreaks-learn/picoed/gccnpl)
## Sample code
```python
from cutebot import *

#Create a sample for Cutebot category
cutebot = Cutebot()    

# While true, detect the status of the line-tracking sensor
# when both detect the black line, the Cutebot is moving forward at 50% speed.
# When the right probe detects that it is off from the black line, set the speed of the left wheel to 0% and the speed of the right wheel to 100%
# When the left probe detects that it is off from the black line, set the left wheel speed to 100% and the right wheel speed to 0%
while True:
    tracing = cutebot.get_tracking()
    if tracing == '11':
        cutebot.set_speed(50,50)
    if tracing == '10':
        cutebot.set_speed(0,100)
    if tracing == '01':
        cutebot.set_speed(100,0)
```
### Code details

1. Import the modules that we need for the program：`cutebot` module contains classes and functions that operate on the Cutebot smart car.
```python
from cutebot import *
```

2. Create a sample for Cutebot category.
```python
cutebot = Cutebot()
```

3. While true, detect the status of the line-tracking sensor, when both detect the black line, the Cutebot is moving forward at 50% speed; when the right probe detects that it is off from the black line, set the speed of the left wheel to 0% and the speed of the right wheel to 100%; when the left probe detects that it is off from the black line, set the left wheel speed to 100% and the right wheel speed to 0%. 

```python
while True:
    tracing = cutebot.get_tracking()
    if tracing == 11:
        cutebot.set_speed(50,50)
        if tracing == 10:
            cutebot.set_speed(0,100)
            if tracing == 01:
        cutebot.set_speed(100,0)
```
## Results
After turning on the power, the Cutebot smart car drives along the black line.
## Exploration
Is it possible to use the Cutebot to make a cart that can prevent falls?
