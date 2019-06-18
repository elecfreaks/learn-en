# 案例05:自动车大灯

## 目的
---
- 让你的Cute:bot智能赛车在黑暗中自动打开车头灯，照亮前方道路。

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

- 在`On start`(开始)积木块中全速前进；
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_05_01.png)

### 步骤 3

- 在`forever`(永久循环)积木块中插入判断积木块，判断光线值是否小于`10`，当小于`10`的时候，左右车灯RGB值全设为`255`，(组合光为白光)。
- 当大于`10`的时候，设置左右车灯RGB值为`0`，关闭车灯。
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_05_02.png)


### 程序

请参考程序连接：[https://makecode.microbit.org/_EYaDJkH4WCff](https://makecode.microbit.org/_EYaDJkH4WCff)

你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_EYaDJkH4WCff" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  
---

## 结论
---
- 当小车经过黑暗的地方，车灯自动点亮，离开黑暗区，车灯自动关闭。

## 思考
---
- 如何编程让小车再每次经过黑暗区的时候，车灯都能亮起不同的颜色。(RGB值控制颜色)

## 常见问题
---
## 相关阅读  
---