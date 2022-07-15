Picoe:ed包含一个17x7的LED点阵屏。
## 属性
### `display`
类[Display](#okDdW)的实例，表示Pico:ed板载的LED点阵屏。
## 类
### `class Display`
用来表示一个由IS31FL3731驱动的点阵屏，在Pico:ed内部使用，用来生成display实例。
> `**clear()**`

清除屏幕

> `**pixel(self, x, y, color=None, blink=None, frame=None)**`

设置x、y 像素闪烁或亮度

- **x - **水平像素位置
- **y - **垂直像素位置
- **color - **像素亮度(0~255)
- **blink - **设置为True，则闪烁该像素
- **frame - **设置像素的帧数

> `**scroll(value, brightness=30)**`

滚动显示字符串或数字

- **value - **要显示的字符串或数字
- **brghtness - **显示屏的亮度(0~255)，默认值30
### `class Image`
用来描述一帧点阵图像，并包含一系列内置图像。
> - **value - **图像文本描述，用0～9指定对应位置LED的亮度。格式如下：
> 
'12345678908765432:'
>         '12345678908765432:'
>         '12345678908765432:'
>         '12345678908765432:'
>         '12345678908765432:'
>         '12345678908765432:'
>         '12345678908765432:'


内置图像列表如下：

- NO
- SQUARE
- RECTANGLE
- RHOMBUS
- TARGET
- CHESSBOARD
- HAPPY
- SAD
- YES
- HEART
- TRIANGLE
- CHAGRIN
- SMILING_FACE
- CRY
- DOWNCAST
- LOOK_RIGHT
- LOOK_LEFT
- TONGUE
- PEEK_RIGHT
- PEEK_LEFT
- TEAR_EYES
- PROUD
- SNEER_LEFT
- SNEER_RIGHT
- SUPERCILIOUS_LOOK
- EXCITED
## 示例
1.显示字符串和数字
```python
import time
from picoed import display

# 静态显示3个字母
display.scroll("ABC")
time.sleep(1)

# 滚动显示数字
display.scroll(1234567890)

# 滚动显示字符串
display.scroll("Hello, world!")

```

2.显示方框
```python
from picoed import display

# 在屏幕上画一个方框
# 首先绘制顶部和底部边缘
for x in range(display.width):
    display.pixel(x, 0, 50)
    display.pixel(x, display.height - 1, 50)
# 现在绘制左右边缘
for y in range(display.height):
    display.pixel(0, y, 50)
    display.pixel(display.width - 1, y, 50)

```

3.显示内置图像
```python
from picoed import display, Image

display.show(Image.HAPPY)

```

4.显示自定义图像
```python
from picoed import display, Image

while True:
    display.show(Image(
        '12345678987654321:'
        '12345678987654321:'
        '12345678987654321:'
        '12345678987654321:'
        '12345678987654321:'
        '12345678987654321:'
        '12345678987654321:'
    ))
    display.show(Image(
        '87654321112345678:'
        '87654321112345678:'
        '87654321112345678:'
        '87654321112345678:'
        '87654321112345678:'
        '87654321112345678:'
        '87654321112345678:'
    ))

```
### 
#### 
