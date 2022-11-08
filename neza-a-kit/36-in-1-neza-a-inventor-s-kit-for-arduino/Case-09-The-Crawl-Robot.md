# Case 09: The Crawl Robot

## Purpose
---
Make a crawl robot with [NezhaA Inventor's Kit](https://shop.elecfreaks.com/products/elecfreaks-arduino-36-in-1-nezha-a-inventors-kit?_pos=2&_sid=e1dfa3343&_ss=r).

![](./images/neza-a-case-09-01.png)

## Purchse
---
 [NezhaA Inventor's Kit](https://shop.elecfreaks.com/products/elecfreaks-arduino-36-in-1-nezha-a-inventors-kit?_pos=2&_sid=e1dfa3343&_ss=r)

## Materials Required
---
![](./images/neza-a-case-09-02.png)

## Assembly Steps
---
![](./images/neza-a-step-09-01.png)
![](./images/neza-a-step-09-02.png)
![](./images/neza-a-step-09-03.png)
![](./images/neza-a-step-09-04.png)
![](./images/neza-a-step-09-05.png)
![](./images/neza-a-step-09-06.png)
![](./images/neza-a-step-09-07.png)
![](./images/neza-a-step-09-08.png)
![](./images/neza-a-step-09-09.png)
![](./images/neza-a-step-09-10.png)
![](./images/neza-a-step-09-11.png)
![](./images/neza-a-step-09-12.png)
![](./images/neza-a-step-09-13.png)
![](./images/neza-a-step-09-14.png)
![](./images/neza-a-step-09-15.png)
![](./images/neza-a-step-09-16.png)
![](./images/neza-a-step-09-17.png)
![](./images/neza-a-step-09-18.png)
![](./images/neza-a-step-09-19.png)
![](./images/neza-a-step-09-20.png)
![](./images/neza-a-step-09-21.png)
![](./images/neza-a-step-09-22.png)
![](./images/neza-a-step-09-23.png)
![](./images/neza-a-step-09-24.png)
![](./images/neza-a-step-09-25.png)
![](./images/neza-a-step-09-26.png)

## Hardware Connections
---
Connect the [motor](https://www.elecfreaks.com/geekservo-motor-2kg-compatible-with-lego.html) to M1 port on [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html). 

![](./images/neza-a-case-09-03.png)

## Programming
---
### Prepare the programming

Steps for preparation please refer to: [Arduino 3 in 1 Breakout Board](https://www.elecfreaks.com/learn-en/Arduino-3-in-1-box/Arduino-3-in-1-box.html).

### Sample Code: 

```
// Language ArduinoC
#include <NezhaA.h>

NezhaA nezhaA;    //Create an instance of Nezha category

void setup() {
  nezhaA.begin();    //Initiliaze the buzzer, motor, servo and light
  nezhaA.setMotorSpeed(M1, 100);    // Set the speed of the motor connecting to M1 at 100%
}

void loop() {

}

```
### Result
After powering on, the robot crawls forward. 
