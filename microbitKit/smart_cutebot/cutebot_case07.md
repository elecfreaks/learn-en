# 案例07:防跌落小车

## 目的
---
- 让你的Cute:bot智能赛车完成最基本的前进后退。

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

- 在`On start`(开始)积木块中显示一个图标。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_07_01.png)

### 步骤 3

- 在`forever`(永久循环)积木块中插入`if`(判断)积木块，判断巡线模块不是两个都检测到(边缘)黑线时，设置左右轮速度为`20`。
- 如果不是，设置左右轮速度为`-50`迅速倒车离开桌面边缘，延迟`300ms`，左轮不动，右轮随机一个50~100的速度旋转`100ms`。
- 然后将左右轮速度设置为`0`，暂停一秒，重新前进。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_07_02.png)

### 程序

请参考程序连接：[https://makecode.microbit.org/_LvweWCb3J72u](https://makecode.microbit.org/_LvweWCb3J72u)

你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_LvweWCb3J72u" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  
---

## 结论
---
- 小车检测到桌面边缘时会迅速后退，然后换一个方向继续前进。

## 思考
---

## 常见问题
---
## 相关阅读  
---