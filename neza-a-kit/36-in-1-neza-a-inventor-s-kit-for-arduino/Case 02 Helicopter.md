# Case 02: Helicopter 
## Purpose
Make a helocopter with [NezhaA Inventor's Kit](https://www.elecfreaks.com/elecfreaks-nezha-a-inventor-s-kit-for-arduino.html). 
![](./images/neza-a-case-02-01.png)

## Purchase 
 [NezhaA Inventor's Kit](https://www.elecfreaks.com/elecfreaks-nezha-a-inventor-s-kit-for-arduino.html)

## Materials Required
![](./images/neza-a-case-02-02.png)
## Assembly Steps
![](./images/neza-a-step-02-01.png)
![](./images/neza-a-step-02-02.png)
![](./images/neza-a-step-02-03.png)
![](./images/neza-a-step-02-04.png)
![](./images/neza-a-step-02-05.png)
![](./images/neza-a-step-02-06.png)
![](./images/neza-a-step-02-07.png)
![](./images/neza-a-step-02-08.png)
![](./images/neza-a-step-02-09.png)
![](./images/neza-a-step-02-10.png)
![](./images/neza-a-step-02-11.png)
![](./images/neza-a-step-02-12.png)
![](./images/neza-a-step-02-13.png)
![](./images/neza-a-step-02-14.png)
![](./images/neza-a-step-02-15.png)
![](./images/neza-a-step-02-16.png)
![](./images/neza-a-step-02-17.png)
![](./images/neza-a-step-02-18.png)
![](./images/neza-a-step-02-19.png)
![](./images/neza-a-step-02-20.png)
![](./images/neza-a-step-02-21.png)
![](./images/neza-a-step-02-22.png)
![](./images/neza-a-step-02-23.png)
![](./images/neza-a-step-02-24.png)
![](./images/neza-a-step-02-25.png)
![](./images/neza-a-step-02-26.png)
![](./images/neza-a-step-02-27.png)
![](./images/neza-a-step-02-28.png)
![](./images/neza-a-step-02-29.png)
![](./images/neza-a-step-02-30.png)
![](./images/neza-a-step-02-31.png)
## Hardware Connections
Connect [Motor](https://www.elecfreaks.com/geekservo-motor-2kg-compatible-with-lego.html) to M1 on [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html). 
![](./images/neza-a-case-02-03.png)

## Programming
### Prepare the programming

Steps for preparation please refer to: [Arduino 3 in 1 Breakout Board](https://www.elecfreaks.com/learn-en/Arduino-3-in-1-box/Arduino-3-in-1-box.html)

### Sample Projects:
```
// Language ArduinoC
#include <NezhaA.h>

NezhaA nezhaA;    //Create an instance of Nezha Catogory

void setup() {
  nezhaA.begin();    //Initiliaze the buzzer, motor, servo and light
  nezhaA.setMotorSpeed(M1, 100);    //Set the speed of the motor connecting to M1 at 100%
}

void loop() {

}

```

### Result
After powering on, the propeller starts driving. 
![](./images/neza-a-case-02-04.gif)