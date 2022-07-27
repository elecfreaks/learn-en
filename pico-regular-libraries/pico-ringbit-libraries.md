# Pico-ringbit-library
## Dependencies
- [CircuitPython](https://circuitpython.org/board/elecfreaks_picoed/)
- [CircuitPython_Motor](https://github.com/adafruit/Adafruit_CircuitPython_Motor)
- [CircuitPython_NeoPixel](https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel)
## Classes
### `class Ringbit(left_pin, right_pin)`
Ringbit class is used to create a ringbit instance

- **left_pin -** left_pin
- **right_pin -** right_pin

> `**set_speed(left_speed, right_speed)**`

Set the speed of left wheel and right wheel

- **left_pin -** Left wheel speed
- **right_pin -**Right wheel speed 

> `**rainbow_leds**`

Create the sample of `class neopixel.NeoPixel`

> `**init_rainbow_leds(pin, n, brightness=1.0, auto_write=True)**`

Initialize the rainbow lights

- **pin -** rainbow pins
- **n -** number of rainbow lights
- **brightness -** Rainbow light brightness (0.0 ~ 1.0)
- **auto_write -** if "True", no need to refresh the rainbow light color by calling  `show()`

> `**get_distance(pin, unit)**`**  **

Get the ultrasonic range distance

- **pin -** Connect the signal pin of the ultrasonic sensor
- **unit -** distance unit, parameter enumeration: `Unit.cm`, `Unit.inch`

> `**get_tracking(pin)**`

Get the status of the line tracking sensor, `'11' `means all in black, `'10' `means black on the left and white on the right, `'01'` means white on the left and black on the right, `'00'` means all in white.

- **pin -** Connect the signal pins of the line tracking sensor
## Example
Set the left and right wheel speed
```python
import board
from ringbit import *

ringbit = Ringbit(board.P0, board.P1)
ringbit.set_speed(50, 50)
```

Rainbow LED
```python
import board
from ringbit import *

ringbit = Ringbit(board.P1, board.P2)

# Initialize the rainbow LED
ringbit.init_rainbow_leds(board.P0, 2)
#  Set light 0 to red, color value in hexadecimal form
ringbit.rainbow_leds[0] = 0xff0000
#  Set light 1 to green in rgb format
ringbit.rainbow_leds[1] = (0, 255, 0)
```
Read ultrasonic distance
```python
import board
import time
from ringbit import *

ringbit = Ringbit(board.P0, board.P1)

while True:
    print(ringbit.get_distance(board.P2, Unit.cm))
    time.sleep(0.5)
```

Read the status of the line-tracking sensor
```python
import board
import time
from ringbit import *

ringbit = Ringbit(board.P0, board.P1)

while True:
    print(ringbit.get_tracking(board.P2))
    time.sleep(0.5)
```



