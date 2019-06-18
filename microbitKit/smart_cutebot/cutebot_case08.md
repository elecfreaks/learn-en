# 案例08:沿着黑线行驶

## 目的
---
- 让你的Cute:bot智能赛车完成寻黑线绕圈跑。

## 使用材料
---
- 1 x [Cutebot套件](https://www.elecfreaks.com/store/cute-bot.html)
- 1 x 巡线地图(自制或使用Cutebot套装内地图)

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

- 在`On start`(开始)积木块中显示图标，选择一颗心；
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_01_02.png)

### 步骤 3

- 在`Forever`(永久循环)积木块中插入三次`if`(判断)积木块。
- 首先判断巡线头状态是否为 ○ ● ，即左巡线头未检测到黑线，右巡线头检测到黑线。
- 将左轮速度设置为`50`，右轮速度`25`，利用速度差完成右转，回归黑线道路。
- 再判断巡线头是否为 ● ○ ，左转回归黑线。
- 当巡线头为 ● ● ，证明小车在黑线上，以`50`的速度直行。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_06_01.png)


### 程序

请参考程序连接：[https://makecode.microbit.org/_brF6tzUKwess](https://makecode.microbit.org/_brF6tzUKwess)

你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_brF6tzUKwess" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  
---

## 结论
---
- 小车按照地图黑线匀速前进，偏离黑线会保持速度和方向行驶，直到回归黑线。

## 思考
---
- 如何在Cutebot自带地图外侧的白圈内行驶而不驶出地图。

## 常见问题
---
## 相关阅读  
---