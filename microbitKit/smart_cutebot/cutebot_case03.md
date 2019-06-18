# 案例03:8字舞蹈
## 目的
---
- 让你的Cute:bot智能赛车沿着8字轨迹运行。
- Cutebot智能赛车是通过左右轮的速度差来完成转向的，是一个三轮车。

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

### 步骤 4

- 在`Forever`(永久循环)积木块中依次插入`全速前进`和`设置左右轮速度`积木块。
- 将8轨迹分为6段，先直行200ms，设置左轮速度大于右轮速度，完成右转1000ms，然后直行200ms，完成8字的上半段小圆圈。
- 同理，完成下半圆

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_03_01.png)

### 程序

请参考程序连接：[https://makecode.microbit.org/_EPpWzRUqwAHA](https://makecode.microbit.org/_EPpWzRUqwAHA)

你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_EPpWzRUqwAHA" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  
---

## 结论
---
- 小车以8字的轨迹行进。

## 思考
---
- 如果想要让小车以一个正方形轨迹行驶，如何编程。

## 常见问题
---
## 相关阅读  
---