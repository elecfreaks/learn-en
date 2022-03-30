# Drone:bit-python使用示例

## 添加python文件

为了方便的使用python对Drone:bit进行编程，我们可以使用已经编写好的库[EF_Produce_MicroPython-master](https://github.com/elecfreaks/EF_Produce_MicroPython/archive/refs/heads/master.zip)，只需要调用函数并修改参数即可实现对应的功能。

下载压缩包并解压[EF_Produce_MicroPython-master](https://github.com/elecfreaks/EF_Produce_MicroPython/archive/refs/heads/master.zip)

打开[Python editor](https://python.microbit.org/v/2.0)

![](./images/AI-py-01.png)

为了给Drone:bit编程，我们需要添加Drone:bit的软件库文件Dronebit.py。点击Load/Save，然后点击Show Files（1）下拉菜单。


![](./images/AI-py-02.png)

再点击Add file在本地找到下载并解压完成的EF_Produce_MicroPython-master文件夹，从中选择Dronebit.py这个文件添加进来。

![](./images/AI-py-03.png)

Dronebit.py添加完成后。

![](./images/AI-py-04.png)

## API

`DRONE(object)`

创建对象。


`heartbeat(self)`

心跳函数，在程序运行过程中保持microbit与无人机的连接，每隔一秒发送一次心跳指令，在程序中需要包含在主循环中。


`Drone_sleep(self,time_ms)`

延时函数，用于代替sleep()，内含心跳指令。


`initModule(self,mode)`

初始化Drone:bit，检查电量，选择模式，初始化完毕会有提示音。

`mode`选择无人机模式：

        `DRONE.master`主控模式，
        `DRONE.remote`遥控模式。


`UAV_speed(self,power)`

动力设定，即无人机速度设定。


`Basic_action(self,basicstate)`

执行基础动作，含起飞和降落功能。

`basicstate`动作指令：

        `DRONE.take_off`起飞，
        `DRONE.take_off`降落。 
        

`Move_action(self,Directionstate,distance)`

执行移动指令。

`Directionstate`动作指令：

        `DRONE.Up`上升，
        `DRONE.Down`下降，
        `DRONE.Forward`前进，
        `DRONE.Backward`后退，
        `DRONE.Left`左侧飞，
        `DRONE.Right`右侧飞；
        
`distance`移动距离：

        单位：厘米，
        上升：0~200，
        下降：0~200，
        其余动作：0~500。


`Rotation_action(self,rotationstate,angle)`执行旋转指令。

`rotationstate`动作指令：

        `DRONE.turn_left`左转，
        `DRONE.turn_right`右转；
        
`angle`旋转角度：

        取值范围：0~360。


`Hovering(self,time)`设置无人机悬停时间。

`time`悬停时间：

        取值范围：0~200。


`Get_voltage(self)`

获取无人机当前电压。


`Get_height(self)`

获取无人机当前高度。



## 示例代码
```
from microbit import *
from Dronebit import *

Drone = DRONE()
Drone.initModule(Drone.master)
Drone.Basic_action(Drone.take_off)
Drone.Move_action(DRONE.Up,300)
Drone.Drone_sleep(1000)
Drone.Move_action(DRONE.Down,300) 
Drone.Drone_sleep(1000)
Drone.Basic_action(Drone.landing)

while True:
    Drone.heartbeat()
    if button_a.was_pressed():
        Drone.Basic_action(Drone.take_off)
        Drone.Move_action(Drone.Forward,300)
        Drone.Drone_sleep(1000)
        Drone.Move_action(Drone.Left,300)
        Drone.Drone_sleep(1000)
        Drone.Move_action(Drone.Backward,300)
        Drone.Drone_sleep(1000)
        Drone.Move_action(Drone.Right,300)
        Drone.Drone_sleep(1000)
        Drone.Hovering(10)
        Drone.Basic_action(Drone.landing)

```
### 结果
- 开机之后，无人机自动起飞并上升、下降、降落，当无人机降落成功后，按下micro:bit的按键A，则无人机会起飞并按正方形轨迹飞行，然后自动降落。
