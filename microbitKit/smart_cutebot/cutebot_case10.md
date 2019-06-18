# 案例10:定距跟车

## 目的
---
- 让你的Cute:bot智能赛车动态运行在一个和你的手固定距离位置上。

## 使用材料
---
- 1 x [Cutebot套件](https://www.elecfreaks.com/store/cute-bot.html)
- 1 x 超声波探头(自备或使用Cutebot套装内探头)

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

- 在`On start`(开始)积木块中插入设置左右轮速度积木块；

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_10_01.png)

### 步骤 3

- 在`Forever`(永久循环)积木块中设置一个`Sonar`变量，用来保存超声波返回的`Cm`值。
- 当超声波返回值大于`5`并且小于`10`时候，位置刚好小车停止。
- 再判断超声波返回值小于`5`的时候，小车距离手太近了，后退。
- 如果都不是，则距离手太远了，前进追上手并且保持位置停止。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_10_02.png)


### 程序

请参考程序连接：[https://makecode.microbit.org/_gRtPkmP0q0cM](https://makecode.microbit.org/_gRtPkmP0q0cM)

你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_gRtPkmP0q0cM" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  
---

## 结论
---
- 小车距离手太远会前进靠近，太近会原理，当距离合适的时候就停止。

## 思考
---

## 常见问题
---
## 相关阅读  
---