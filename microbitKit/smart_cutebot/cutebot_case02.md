# 案例02:均匀加速

## 目的
---
- 完成上一个案例，大家会发现，后驱的Cutebot车速非常快，以至于在起步的时候，前万向轮会离开地面。
- 本案例我们均匀的加速，完成一个平稳的起步。

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
- 并且将速度变量`speed`设置为0，意味着初始速度为0。
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_02_01.png)

### 步骤 3

- 在`Forever`(无限循环)积木块中插入设置左右轮速度积木块，将速度值设置为`speed`，然后将`speed`加一。
- 并且判断如果`speed`速度等于`100`的时候，速度已经为最大值，将速度`speed`设置为0，重新起步。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_01_02.png)

### 程序

请参考程序连接：[https://makecode.microbit.org/_6X6aA3cKKMAt](https://makecode.microbit.org/_6X6aA3cKKMAt)

你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_4uqbF8U6XhWz" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  
---

## 结论
---
- 小车循环完成匀速起步，不会因为车速过快使前轮离地。

## 思考
---
- 如何编写让小车匀加速后匀减速。

## 常见问题
---
## 相关阅读  
---