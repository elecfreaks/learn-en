# Smart Cutebot Samples for Python

---


### Add Python File
Download to unzip it: [EF_Produce_MicroPython-master](https://github.com/lionyhw/EF_Produce_MicroPython/archive/master.zip)
Go to  [Python editor](https://python.microbit.org/v/2.0)

![](./images/cutebot-py-01.png)

We need to add Cutebot.py for programming. Click "Load/Save" and then click "Show Files (1)" to see more choices, click "Add file" to add Cutebot.py from the unzipped package of EF_Produce_MicroPython-master. 

![](./images/cutebot-py-02.png)
![](./images/cutebot-py-03.png)
![](./images/cutebot-py-04.png)

### Samples
### Sample 1: Drive the car at a full speed. 
```
from microbit import *
from Cutebot import *
ct = CUTEBOT()
ct.set_motors_speed(100, 100)

```
### Result
- The speed of the left and right wheels is at 100, the car moves forward at the full speed. 


### Sample 2: Turn the headlights on
```
from microbit import *
from Cutebot import *
ct = CUTEBOT()
ct.set_car_light(left, 0, 90, 90)
ct.set_car_light(right, 200, 200, 0)
```
### Result
- The two headlights light up in different colours. 

### Sample 3: Obstacles avoidance 
```
from microbit import *
from Cutebot import *

dis = CUTEBOT()

while(True):
    i = dis.get_distance(0)
    if i>3 and i<20:
        dis.set_motors_speed(-50, 50)
        sleep(500)
    else:
        dis.set_motors_speed(50, 50)
```
### Result
- The Cutebot turns its direction once it detects any obstacle ahead of it. 

### Sample 4: Line-tracking 
```
from microbit import *
from Cutebot import *

dis = CUTEBOT()

while(True):
    i = dis.get_tracking()
    if i == 10:
        dis.set_motors_speed(10, 50)
    if i == 1:
        dis.set_motors_speed(50, 10)   
    if i == 11:
        dis.set_motors_speed(25, 25)  
```
### Result

- The Cutebot drives along with the black line. 

### Sample 5:  Control the servo  
```
from microbit import *
from Cutebot import *

dis = CUTEBOT()

while(True):
    dis.set_servo(0,180)
    sleep(1000)
    dis.set_servo(0,0)
    sleep(1000)
```
### Result
- The servo connecting to S1 continues driving back and forth. 

## Relevant Case
---

## Technique File
---
