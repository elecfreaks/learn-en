# The first part: Upload the data collected by IoT kit to the Thingspeak IoT platform.

ThingSpeak can deal with HTTP request, save and process data. This platform has function as open application, real-time data collection, location data, data processing, visualization, device status information and plug-in. It can integrate many hardwares and software platforms like Arduino, Raspberry Pi, ioBridge/RealTime.io、Electic lmp, mobile & internet application, social network and MATLAB data processing. It also porvide hosted service apart from open source edition.

Thingspeak link: [thingspeak](https://thingspeak.com/)

## Thingspeak Registration
---
Head to thingspeak website, click on Get Started For Free and in create MathWorks Account package.

![](./images/case_ts_01.png)

- Fill in the registration information and click continue to go on.（As below）

![](./images/case_ts_02.png)

- Confirm the email address, click it as the sign in account to continue.

![](./images/case_ts_03.png)

- Verify your MathWorks account and the thingspeak will send an email to your email box. You need to click the lin of the email to verify and continue. 

![](./images/case_ts_04.png)
 
- Then set your own user ID and password(Note: both Captital and lower case words are required)，then click on continue to go on.

![](./images/case_ts_05.png)

- Then, Sign-up successful!

![](./images/smC48sY.png)

![](./images/case_ts_06.png)

## Thingspeak guide:
---
- Here we will upload luminous intensity for testing. 

- Click on “MY Channels” and click on **New Channel** for your new project.

!![](./images/case_ts_07.png)

- An project parameter design list be showed. If there are more parameters, you need to choose more fields.

![](./images/case_ts_08.png)

- Then, click on save channel. 

- But here you will find nothing. You can find the data of what we have uploaded here:
- 
![](./images/case_ts_09.png)

- Click on API KEY, parameters as below be showed.

![](./images/case_ts_10.png)

## Coding
---

### Connection diagram:
- Connect the iot:bit to the micro:bit.
- 
![](./images/case_ts_17.png)

#### Step 1
- Click on "Advanced" in the MakeCode drawer to see more code selections.

![](./images/iot_bit_11.jpg)

- We need to add an extension for coding to the IOT. Click on the “Extension” at bottom of coding drawer, then search for “IOT” and click on the IOT package to add it to your project. (As below picture) 

![](./images/iot_bit_12.jpg)

***Note：*** If you get a warning telling you some packages will be removed because of incompatibility issues, either follow the prompts or create a new project in the Project file menu.

#### Step 2

Drag the `set 8266` block into the `on start` and choose RX`P8`TX`P12` `baud rate`115200`.

Snap into the `connect wifi` block，write in your wifi name and the key. 

![](./images/case_ts_11.png)

***Note：*** The 8266 module can't support the 5G, please conenct it to 2.4G

#### Step 3

Snap `connect thinkspeak`, `set data` and "upload data to Thingspeak"  into the `forever`. 

Write `write api key` into `set data` and snap the randow number block to the field1.


![](./images/case_ts_12.png)



#### Program

program link：[https://makecode.microbit.org/_0MqJdw99D2hV](https://makecode.microbit.org/_0MqJdw99D2hV)

If you don't want to type these code by yourself, you can directly download the whole program from the link below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_0MqJdw99D2hV" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


#### Result

Uploading the random data to the thingspeak continuously. 

You can check all datas on the thingspeak.

![](./images/case_ts_13.png)


## Thingspeak Add visulization
---
- Click the visulization button to choose the three choices: [stopwatch],[Numeric Display],[Threshold indicator light].

![](./images/case_ts_14.png)

![](./images/case_ts_15.png)

- Choose types of the stopwatch and click NEXT, write the name, filed, the maximum and minimum value of the chart, then click Create to create a new chart.

![](./images/case_ts_16.png)

Both the chart and the value of Field 1 changed.

![](./images/case_ts_19.png)

- Add the numeric display and Threshold indicator light in the same way for the chart.

![](./images/case_ts_20.png)
