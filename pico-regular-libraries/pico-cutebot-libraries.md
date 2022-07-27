# Pico-cutebot-library
## Dependencies
- [CircuitPython](https://circuitpython.org/board/elecfreaks_picoed/)
- [CircuitPython_IRRemote](https://github.com/adafruit/Adafruit_CircuitPython_IRRemote)
- [CircuitPython_NeoPixel](https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel)
## Classes
### `class Cutebot()`
Cutebot class is used to create a Cutebot instance

> `**set_speed(left_speed, right_speed)**`

Set the left wheel and right wheel speed

-  **left_speed -** Left wheel speed, parameter range: -100~100
- **right_speed -** Right wheel speed, parameter range: -100~100

> `**set_light(light_num, rgb_r, rgb_g, rgb_b)**`

Set the left and right wheel speed

- **light_num -** Select RBG light, parameter enumeration: `RGB.left`, `RGB.right`
- Red light value, parameter range: 0~255
- Green light value, parameter range: 0~255
-  Blue light value, parameter range: 0~255

> `**get_distance(unit:Unit)**`

Get ultrasonic range distance

- **unit -** distance unit, parameter enumeration: `Unit.cm`, `Unit.inch`

> `**get_tracking()**`

Get the status of the line tracking sensor, `'11' `  means all in black, `'10' ` means black on the left and white on the right, `'01'` means white on the left and black on the right, `'00'` means all in white.

> `**set_servo(servo_num:Servo, angle)**`

Set the servo angle

- **servo_num -**   select servo, parameter enumeration: `Servo.s1`, `Servo.s2`
- **angle  -** Servo angle, parameter range: 0~180

> `**get_ir_value()**`

Get IR remote key value, return value 0~19, 100, 200

> `**rainbow_leds**`

Create the sample of `class neopixel.NeoPixel` .

> `**init_rainbow_leds(brightness=1.0, auto_write=True)**`

Initialize rainbow led

- **brightness -**rainbow lights brightness (0.0 ~ 1.0)
- **auto_write -** If "True",  no need to refresh the rainbow light color by calling `show()`.

## Example
Set the speed of the cart
```python
from cutebot import *

cute = Cutebot()
cute.set_speed(50, 50)
```

Light up the RGB lights
```python
from cutebot import *

cute = Cutebot()

cute.set_light(RGB.left,80,120,230)
cute.set_light(RGB.right,250,130,60)
```

Get ultrasonic detection distance
```python
import time
from cutebot import *

cute = Cutebot()

while True:
    if button_a.is_pressed():
        print(cute.get_distance(Unit.cm))
        time.sleep(0.5)
```

Get the status of the line tracking sensor
```python
import time
from cutebot import *

cute = Cutebot()

while True:
    if button_a.is_pressed():
        print(cute.get_tracking())
        time.sleep(0.5)
```

Set the angle of the servos
```python
from cutebot import *

cute = Cutebot()

cute.set_servo(Servo.s1,120)
cute.set_servo(Servo.s2,150)
```

Get IR remote key value
```python
from cutebot import *

cute = Cutebot()

while True:
    print(cute.get_ir_value())
```

Rainbow led
```python
from cutebot import *

cute = Cutebot()

# Initialize the rainbow lights
cute.init_rainbow_leds()
#  Set light 0 to green, color value hexadecimal form
cute.rainbow_leds[0] = 0x00ff00
#  Set light 1 to blue in rgb form
cute.rainbow_leds[1] = (0, 0, 255)
```



