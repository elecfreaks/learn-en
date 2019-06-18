# 案例04:随便跑跑

## 目的
---
- 让你的Cute:bot智能赛车像是有思维一样，以他的想法前进，后退转向等。

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

- 在`On start`(开始)积木块中显示图标，选择一颗心；
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_01_02.png)

### 步骤 3

- 在`forever`(永久循环)积木块中设置两个变量`left_speed`和`right_speed`，用于控制左右轮的速度，分别生成`-100`到`100`的随机数赋值到这两个变量里。
- 然后将左右轮速度设置为这两个变量。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_04_01.png)


### 程序

请参考程序连接：[https://makecode.microbit.org/_UFETasLycR3g](https://makecode.microbit.org/_UFETasLycR3g)

你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_UFETasLycR3g" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  
---

## 结论
---
- 小车随机前进，后退或者转向。

## 思考
---

## 常见问题
---
## 相关阅读  
---