# 板载LED
Pico:ed包含一颗板载LED灯。该LED灯是固件状态指示灯，当复位时会快速闪烁数次，当程序空闲时会每隔5秒亮一次，同时这颗LED灯可以编程控制。
## 属性
### `led`
类[Led](#d1QQW)的实例，表示板载LED灯。
## 类
### `class Led(pin)`
用来表示一颗LED灯。

- **pin -**  Led引脚

> `**on**`

打开LED。

> `**off()**`

关闭LED。

> `**toggle()**`

切换LED状态。

> `**deinit()**`

Deinit LED，释放引脚。
## 示例
1.blink1
```python
import time
from picoed import *

while True:
    led.on()
    time.sleep(0.5)
    led.off()
    time.sleep(0.5)
```

2.blink2
```python
import time
from picoed import *

while True:
    led.toggle()
    time.sleep(0.5)
```

## 



