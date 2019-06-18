# 案例06:转向示廓灯

## 目的
---
- 让你的Cute:bot智能赛车转弯时开启转向灯和转向示廓灯。

## 使用材料
---
- 1 x [Cutebot套件](https://www.elecfreaks.com/store/cute-bot.html)

## 软件平台
---
[微软 makecode](https://makecode.microbit.org/#)

## 编程
---
### 步骤 1
- 在MakeCode的代码抽屉中点击Advanced，查看更多代码选项。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot-pk-1.png)

- 为了给Cutebot套件编程，我们需要添加一个代码库。在代码抽屉底部找到“Add Package”，并点击它。这时会弹出一个对话框。搜索`Cutebot`，然后点击下载这个代码库。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/cutebot-pk-11.png)

注意：如果你得到一个提示说一些代码库因为不兼容的原因将被删除，你可以根据提示继续操作，或者在项目菜单栏里面新建一个项目。

### 步骤 2

- 在`On start`(开始)积木块中设置Rainbow LED灯连接口为`P15`，一共有`2`颗LED灯；
- `right`右侧灯为从第`0`颗灯开始往后`1`颗灯。
- `left`左侧灯为从第`1`颗灯开始往后`1`颗灯。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_06_01.png)

### 步骤 3

- 在`on button A pressed`(当按钮A按下时)积木块中插入`repeat`(循环)积木块，右侧示廓灯显示黄色，左侧LED大灯显示黄色(RGB控制)，延迟500ms后，关闭左侧示廓灯和LED大灯，完成一次闪烁。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_06_02.png)


### 步骤 4

- 在`on button B pressed`(当按钮B按下时)积木块中与右侧同理，只不过将右侧改为左侧。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_06_03.png)

### 程序

请参考程序连接：[https://makecode.microbit.org/_FzDFDbCcHfvP](https://makecode.microbit.org/_FzDFDbCcHfvP)

你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_4uqbF8U6XhWz" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  
---

## 结论
---
- 当按钮A按下时，右侧LED车灯和示廓灯闪烁5次
- 当按钮B按下时，左侧LED车灯和示廓灯闪烁5次

## 思考
---
- 如何让你的小车按下按钮A开启双闪，按下按钮B关闭双闪呢。

## 常见问题
---
## 相关阅读  
---