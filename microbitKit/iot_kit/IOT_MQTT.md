# How to Apply with HiveMQ

HiveMQ is an MQTT broker and client-based messaging platform designed to move data in and out of connected IoT devices quickly, efficiently and reliably.

Website: [https://www.hivemq.com/](https://www.hivemq.com/)

## Register
---
Click the "Cloud" button on the page. 

![](./images/IOT_HiveMQ_01.png)

Click "Sign up now". 

![](./images/IOT_HiveMQ_02.png)

 Choose "Sign Up" to register your info(email, passwords). 

![](./images/IOT_HiveMQ_03.png)

Requirements of the passwords. 

![](./images/IOT_HiveMQ_04.png)

Following the guide to complete the registration. 

## Operation Guide
---
After registration, go to: https://www.hivemq.com/mqtt-cloud-broker/
Choose "Sigh up now".

![](./images/IOT_HiveMQ_02.png)

Log in with your email and password. 

![](./images/IOT_HiveMQ_05.png)

Click "CREATE CLUSTER".

![](./images/IOT_HiveMQ_06.png)

Choose "Azure" and click "CREATE CLUSTER".

![](./images/IOT_HiveMQ_07.png)

Click "MANAGE CLUSTER".

![](./images/IOT_HiveMQ_08.png)

Click "Access Management",  set the "Username" and "Password", then click "ADD". （Add the user's account）

![](./images/IOT_HiveMQ_09.png)

Completed! Please remember the user name and the password, this info would be required on the settings of the MQTT in MakeCode. 

![](./images/IOT_HiveMQ_10.png)





For hardware connections, please refer to our wiki: [https://www.elecfreaks.com/learn-en/microbitKit/iot_kit/iot_bit.html](https://www.elecfreaks.com/learn-en/microbitKit/iot_kit/iot_bit.html)

**Attention:** Please use the USB port on the IoT:bit for power supply, or the Wifi module would not get powered. 

Go to MakeCode: [https://makecode.microbit.org/#editor](https://makecode.microbit.org/#editor)

Click "Advanced" in the MakeCode drawer to see more choices, and then click "Extensions".

![](./images/IOT_HiveMQ_11.png)

Search with "iot-environment-kit" to add the extension. 

![](./images/IOT_HiveMQ_12.png)

Choose "ESP8266_IoT".

![](./images/IOT_HiveMQ_13.png)

In the on start block, initialize esp8266 and enter with the name and password of the wifi for connecting. 

![](./images/IOT_HiveMQ_14.png)

 Set the applications of MQTT, set "scheme" as "TSL", self-define "clientID", add the user name and password with the one on HiveMQ. 

![](./images/IOT_HiveMQ_15.png)

Click "Overview" and copy the "Host" and "port" to MakeCode. 

![](./images/IOT_HiveMQ_16.png)

Click "Getting started",  choose "HiveMQ Websocket Client".

![](./images/IOT_HiveMQ_17.png)

In the jumping page, click "here" on step 1. 

![](./images/IOT_HiveMQ_18.png)

In the jumping page, enter with the User and Password, then click "Connect" to get in touch with MQTT . 

![](./images/IOT_HiveMQ_19.png)

A notice of "connected" labled in green occurs if the connection is made successfully. 

Click "Add New Topic Subscription" . 

![](./images/IOT_HiveMQ_20.png)

Choose "Subscribe".

![](./images/IOT_HiveMQ_21.png)

If completed, it is ok to send messages from MakeCode. 

The "hello" in the block is the message we are going to send, you can set it by yourself. And the topic block: "testtopic/1" is the pre-settings on the platform, you can replace "#" with any number. 

![](./images/IOT_HiveMQ_22.png)

Following the former steps, press the button A on micro:bit to send "hello" to the platform. 

![](./images/IOT_HiveMQ_23.png)

Absolutely, we can send data from the platform to local part, set the topic as "testtopic/2", and enter the messages  on "Message", then click "Publish" to send. 
And make sure to keep the topic in the blocks the same. 

![](./images/IOT_HiveMQ_24.png)

Send the number "2" from the platform and display it on the micro:bit. 

![](./images/IOT_HiveMQ_25.png)

Program:

![](./images/IOT_HiveMQ_26.png)

Link: [https://makecode.microbit.org/_2Ys7uE8F7Dr8](https://makecode.microbit.org/_2Ys7uE8F7Dr8)


## FAQ
---
Q: How to judge if the current IoT:bit supports MQTT? 
A: Please refer to the version number printed on the back of the IoT:bit, only V1.6 supports MQTT, V1.4 and the former are not availble for MQTT.

![](./images/IOT_HiveMQ_27.png)
