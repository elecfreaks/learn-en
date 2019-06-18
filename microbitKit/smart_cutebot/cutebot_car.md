# Cutebot智能赛车简介

## 简介  
---

ELECFREAKS Cutebot是一款带有双高速电机马达的后驱智能赛车。

Cutebot同时搭载了很多车载设备，包括超声波导航距离传感器，两颗RGBLED车大灯，两颗Rainbow LED车底示廓灯，两个车道辅助巡线探头，一颗有源蜂鸣车喇叭，和更多智能配件！驱动你的第一个智能赛车吧！

### 产品特性
---

- 高速电机，采用双高速电机后置驱动，动力强劲。
- 结构小巧，采用圆弧造型，边缘防撞，手感舒适。
- 组装方便，只需安装电池组和超声波，方便快捷。
 
## 产品图片
---
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_01.jpg)

## 技术参数
---

|技术类别 |参数|
|:-:|:-:|
|支持电压| 3.5V — 5V |
| 尺寸 |85.68mm X 85.34mm X 38.10mm|
|蜂鸣器|有源蜂鸣器连接至P0口|
|红外遥控|支持接收连接至P16口|
|RGB车头灯|2 x RGB控制|
|Rainbow LED|2 x Neopixel控制连接至P15|
| 接口 |IIC接口(P19,P20)、超声波接口、P1、P2(以GVS端子引出)|
| 电机类型 |GA12-N20微型直流齿轮减速电机(300转/分钟)|
| 超声波类型 |HC-SR04(2cm-400cm非接触式距离感测,精度3mm)|

## 功能模块描述
---
小车正前方配备超声波接口和micro:bit的IIC接口

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_02.jpg)

- - - - -

前方左右两边各配备两颗RGB全彩色LED车灯，通过扩展板控制，不占用micro:bitIO口数量。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_03.jpg)

- - - - -

车辆板载一颗蜂鸣器，连接到micro:bit主板的P0口，可以使用`Music`积木块中的积木来驱动。


![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_13.jpg)

- - - - -

正上方装有三颗AA电池电池盒扩展板，用来驱动整个小车。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_04.jpg)

- - - - -

电池盒扩展板上同时扩展了micro:bit的IIC接口和P1，P2 IO接口。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_05.jpg)

- - - - -

小车尾部带有红外线接收头，连接在micro:bit主板的P16接口。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_06.jpg)

- - - - -

尾部红外线接收头旁边为小车总电源开关，同时配有一颗LED灯指示开关状态。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_07.jpg)

- - - - -

左右两边为两个 微型高速直流齿轮减速电机 驱动的车轮，转速高达(300转/分钟)，享受飞驰一般的速度。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_08.jpg)

- - - - -

小车底部前方有两个巡线头，用于检测黑线及边缘，连接到micro:bit主板的P13和P14接口。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_09.jpg)

- - - - -

小车底部前方装配一个金属万向轮，小车用 左右轮速度差的方式 完成360度全方向行驶。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_10.jpg)

- - - - -

底部两侧边安装了两颗Rainbow LED 全彩灯珠，连接到micro:bit主板的P15口，需要使用扩展`Neopixel`来驱动使用，可以作为小车示廓灯或其他功能使用。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot_01_11.jpg)
## 零件清单
---

- 1 x Cutebot car
- 1 x 电池盒
- 1 x HC-SR04超声波模块
- 1 x 巡线地图
- 1 x 产品手册

## 文档
---

## 常见问题
---
