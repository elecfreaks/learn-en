# pico-ringbit-library
## 依赖
- [CircuitPython](https://circuitpython.org/board/elecfreaks_picoed/)
- [CircuitPython_Motor](https://github.com/adafruit/Adafruit_CircuitPython_Motor)
- [CircuitPython_NeoPixel](https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel)
## 类
### `class Ringbit(left_pin, right_pin)`
Ringbit类，用来创建一个ringbit实例

- **left_pin -** 左轮引脚
- **right_pin -** 右轮引脚

> `**set_speed(left_speed, right_speed)**`

设置左轮和右轮速度

- **left_pin -** 左轮速度
- **right_pin -** 右轮速度 

> `**rainbow_leds**`

`class neopixel.NeoPixel`的实例

> `**init_rainbow_leds(pin, n, brightness=1.0, auto_write=True)**`

初始化彩虹灯

- **pin -** 彩虹灯引脚
- **n -** 彩虹灯的数量
- **brightness -** 彩虹灯亮度(0.0 ~ 1.0)
- **auto_write -** 如果为True，则不用显示调用`show()`刷新彩虹灯颜色

> `**get_distance(pin, unit)**`**  **

获取超声波测距距离

- **pin -** 连接超声波传感器的信号引脚
- **unit -** 距离单位，参数枚举：`Unit.cm`、`Unit.inch`

> `**get_tracking(pin)**`

获取巡线传感器的状态，`11`均在黑色，`10`左黑右白，`01`左白右黑，`00`均在白色

- **pin -** 连接巡线传感器的信号引脚
## 示例
设置左右轮速度
```python
import board
from ringbit import *

ringbit = Ringbit(board.P0, board.P1)
ringbit.set_speed(50, 50)
```

彩虹灯
```python
import board
from ringbit import *

ringbit = Ringbit(board.P1, board.P2)

# 初始化彩虹灯
ringbit.init_rainbow_leds(board.P0, 2)
# 设置0号灯为红色，色值16进制形式
ringbit.rainbow_leds[0] = 0xff0000
# 设置1号灯为绿色，rgb形式
ringbit.rainbow_leds[1] = (0, 255, 0)
```
读取超声波距离
```python
import board
import time
from ringbit import *

ringbit = Ringbit(board.P0, board.P1)

while True:
    print(ringbit.get_distance(board.P2, Unit.cm))
    time.sleep(0.5)
```

读取巡线传感器状态
```python
import board
import time
from ringbit import *

ringbit = Ringbit(board.P0, board.P1)

while True:
    print(ringbit.get_tracking(board.P2))
    time.sleep(0.5)
```



