# pico-cutebot-library
## 依赖
- [CircuitPython](https://circuitpython.org/board/elecfreaks_picoed/)
- [CircuitPython_IRRemote](https://github.com/adafruit/Adafruit_CircuitPython_IRRemote)
- [CircuitPython_NeoPixel](https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel)
## 类
### `class Cutebot()`
Cutebot类，用来创建一个cutebot实例

> `**set_speed(left_speed, right_speed)**`

设置左轮和右轮速度

-  **left_speed -** 左轮速度，参数范围：-100~100
- **right_speed -** 右轮速度，参数范围：-100~100

> `**set_light(light_num, rgb_r, rgb_g, rgb_b)**`

设置左轮和右轮速度

- **light_num -** 选择RBG灯，参数枚举：`RGB.left`、`RGB.right`
- 红色灯光值，参数范围：0~255
- 绿色灯光值，参数范围：0~255
- 蓝色灯光值，参数范围：0~255

> `**get_distance(unit:Unit)**`

获取超声波测距距离

- **unit -** 距离单位，参数枚举：`Unit.cm`、`Unit.inch`

> `**get_tracking()**`

获取巡线传感器的状态，`'11'`均在黑色，`'10'`左黑右白，`'01'`左白右黑，`'00'`均在白色

> `**set_servo(servo_num:Servo, angle)**`

设置舵机角度

- **servo_num -**  选择舵机，参数枚举：`Servo.s1`、`Servo.s2`
- **angle  -** 舵机角度，参数范围：0~180

> `**get_ir_value()**`

获取红外遥控按键值，返回值0~19、100、200

> `**rainbow_leds**`

`class neopixel.NeoPixel`的实例

> `**init_rainbow_leds(brightness=1.0, auto_write=True)**`

初始化彩虹灯

- **brightness -** 彩虹灯亮度(0.0 ~ 1.0)
- **auto_write -** 如果为True，则不用显示调用`show()`刷新彩虹灯颜色
## 示例
设置小车速度
```python
from cutebot import *

cute = Cutebot()
cute.set_speed(50, 50)
```

点亮RGB灯
```python
from cutebot import *

cute = Cutebot()

cute.set_light(RGB.left,80,120,230)
cute.set_light(RGB.right,250,130,60)
```

获取超声波探测距离
```python
import time
from cutebot import *

cute = Cutebot()

while True:
    if button_a.is_pressed():
        print(cute.get_distance(Unit.cm))
        time.sleep(0.5)
```

获取巡线传感器状态
```python
import time
from cutebot import *

cute = Cutebot()

while True:
    if button_a.is_pressed():
        print(cute.get_tracking())
        time.sleep(0.5)
```

设置舵机角度
```python
from cutebot import *

cute = Cutebot()

cute.set_servo(Servo.s1,120)
cute.set_servo(Servo.s2,150)
```

获取红外遥控按键值
```python
from cutebot import *

cute = Cutebot()

while True:
    print(cute.get_ir_value())
```

彩虹灯
```python
from cutebot import *

cute = Cutebot()

# 初始化彩虹灯
cute.init_rainbow_leds()
# 设置0号灯为绿色，色值16进制形式
cute.rainbow_leds[0] = 0x00ff00
# 设置1号灯为蓝色，rgb形式
cute.rainbow_leds[1] = (0, 0, 255)
```



