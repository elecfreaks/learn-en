# FAQ 05
## Q: What do I need to pay attention to when using IOTbit to link MQTT?

A:Please follow the steps in the wiki documentation, link to the documentation:[How to Apply with HiveMQ](http://www.elecfreaks.com/learn-en/microbitKit/iot_kit/IOT_MQTT.html).

**Points to note:**

1. The `clientID` of the program in MakeCode is customizable, but it should be noted that it cannot be the same as the `clientID` of the HiveMQ platform.
 
2.The `port` of the program in MakeCode should be filled in as`8883`.

3.You need to cheek `SSL` on HiveMQ platform.
