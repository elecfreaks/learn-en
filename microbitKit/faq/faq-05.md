# FAQ 05
## Q:使用IOTbit链接MQTT需要注意哪些事项？

A:请根据wiki文档中的步骤进行操作.

文档链接:[How to Apply with HiveMQ](http://www.elecfreaks.com/learn-en/microbitKit/iot_kit/IOT_MQTT.html)。

**注意事项:**

1.makecode中程序的`clientID`是可以自定义的，但是需要注意的不能跟HiveMQ平台的`clientID`相同.

2.makecode中程序的`port`是应该填写为`8883`.

3.HiveMQ平台上需要将`SSL`选中.
