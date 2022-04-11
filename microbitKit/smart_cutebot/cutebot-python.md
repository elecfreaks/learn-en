# Smart Cutebot Samples for Python

---


### Add Python File
Download to unzip it: [EF_Produce_MicroPython-master](https://github.com/elecfreaks/EF_Produce_MicroPython/archive/refs/heads/master.zip)
Go to  [Python editor](https://python.microbit.org/v/2.0)

![](./images/cutebot-py-01.png)

We need to add Cutebot.py for programming. Click "Load/Save" and then click "Show Files (1)" to see more choices, click "Add file" to add Cutebot.py from the unzipped package of EF_Produce_MicroPython-master. 

![](./images/cutebot-py-02.png)
![](./images/cutebot-py-03.png)
![](./images/cutebot-py-04.png)

## API

`CUTEBOT(object)`

创建对象。

`set_motors_speed(self, left_wheel_speed: int, right_wheel_speed: int)`

设置左右轮的电机速度：

        `left_wheel_speed: int`左轮速度-100～100
        `right_wheel_speed: int`右轮速度-100～100。

`set_car_light(self, light: int, R: int, G: int, B: int)`

设置车头灯颜色:

        `light`:选择车灯
        `R`:R通道颜色0-255`
        `G`:G通道颜色0-255`
        `B`:B通道颜色0-255`
        


`get_distance(self, unit: int = 0)`

车头超声波读取距离:

        `unit`检测距离单位:` 0 `厘米,` 1 `英尺
        
         

`get_tracking(self)`

返回当前巡线头状态:

        return:`00` 均在白色
               `10` 左黑右白
               `01` 左白右黑
               `11` 均在黑色
               

`set_servo(self, servo, angle)`

选择伺服电机并且设置角度/速度:

            `servo (number)`选择第几个舵机（伺服电机）1,2
           `angle (number)`设置舵机角度 0~180



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

## FAQ

关于程序报错信息：

 |ValueError|错误内容|
 |:---:|:---:|
 |speed error,-100~100|小车的左轮或者右轮的速度超出设定阈值|
 |RGB is error|小车的车头灯颜色参数超出设定阈值|
 |select servo error,1,2|小车的舵机接口参数设置错误|
 |angle error,0~180|舵机旋转角度设置错误|



## Relevant Case
---

## Technique File
---
