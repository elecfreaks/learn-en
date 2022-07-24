# Onboard LED
Pico:ed includes an onboard LED. This LED is a firmware status indicator that flashes rapidly several times when reset and every 5 seconds when the program is idle, and this LED is programmable.
## Attributes
### `led`
The instance of class [Led](#d1QQW)  represents the onboard LEDs.
## Classes
### `class Led(pin)`
It is to represent an LED.

- **pin -**  Led pins

> `**on**`

Turns on the LED.

> `**off()**`

Turn off the LED.

> `**toggle()**`

Toggle the LED state.

> `**deinit()**`

Deinit the LED and release the pin.
## Example
1. Blink1

```python
import time
from picoed import *

while True:
    led.on()
    time.sleep(0.5)
    led.off()
    time.sleep(0.5)
```

2. Blink2

```python
import time
from picoed import *

while True:
    led.toggle()
    time.sleep(0.5)
```

## 



