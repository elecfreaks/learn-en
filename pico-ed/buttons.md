# Buttons

Pico:ed contains two keys: A and B.
## Attributes
### `button_a`
An instance of a class [Button](#w8UmM) representing the button on the left.
### `button_b`
An instance of a class [Button](#w8UmM) representing the button on the right.
## Classes
### `class Button(pin)`
It is for representing a button.

- **unit -** Button pins

> `**is_pressed()**`

Returns "True" if the button is pressed, otherwise it returns "False".

> `**was_pressed()**`

Returns "True" if the button is pressed and only once before the next press.
## Example
1.Controls the LED

```python
# Import the modules that we need for the program
from picoed import *

#  While true, detect if buton A is pressed and also the status of the LED
while True:
    if button_a.is_pressed():
        led.on()
    else:
        led.off()

```

2. Count the times of pressing the buttons

```python
from picoed import *

times = 0
display.show(times)

while True:
    # Press button A once, count minus 1
    if button_a.was_pressed():
        times -= 1
        display.show(times)
    # Press button_B once, add 1 to the count
    if button_b.was_pressed():
        times += 1
        display.show(times)

```

