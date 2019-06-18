# 案例12:micro:bit加速度计远程控制

## 目的
---
- 使用另一块micorbit加速度计远程操控Cutebot赛车，可以控制小车360度方向和速度。
- 两块主板都需要编程

## 使用材料
---
- 1 x [Cutebot套件](https://www.elecfreaks.com/store/cute-bot.html)
- 1 x [micro:bit主板](https://item.taobao.com/item.htm?spm=a1z10.1-c-s.w5003-18615042388.1.410d58b3rNtft8&id=562621059348&scene=taobao_shop)

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

### 步骤 2: 遥控器编程

- 在`On start`(开始)积木块中设置无线电组别为`1`；
- 在`forever`(无线循环)积木块中无线发送数据`x`它的值为`x轴加速度值`整除`10`。
- 在`forever`(无线循环)积木块中无线发送数据`y`它的值为`y轴加速度值`整除`10`。
- 因为加速度值的范围是`0`~`1024`，整除`10`以后可以近似看为`0`~`100`的速度值。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_12_01.png)

#### 程序

请参考程序连接：[https://makecode.microbit.org/_0Xo6EX0weMVF](https://makecode.microbit.org/_0Xo6EX0weMVF)

你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_0Xo6EX0weMVF" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  

### 步骤 3: 小车编程

- 在`On start`(开始)积木块中设置无线电组别为`1`，一定要和遥控端设置为同一组别，否则无法匹配。
- 然后在`on radio received`积木块中插入两次判断语句，分别判断无线电接收值`name`是否为`x`或者`y`；
- 当无线电收到的`name`值为`x`时，为加速度计`X`轴数据，将`value`值保存到`xValue`变量；
- 当无线电收到的`name`值为`y`时，为加速度计`Y`轴数据，将`value`值保存到`yValue`变量；
- 在`forever`(无限循环)积木块中，设置左轮速度为`yValue`+`xValue`，右轮速度为`yValue`-`xValue`。

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/smart_cutebot/images/case_12_02.png)

#### 程序

请参考程序连接：[https://makecode.microbit.org/_6ExC8oRz3i6U](https://makecode.microbit.org/_6ExC8oRz3i6U)

你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_6ExC8oRz3i6U" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  

## 结论
---
- micro:bit控制主板向某一个方向倾斜控制Cutebot小车的前进方向。
- 控制端的倾斜角度控制Cutebot小车的车速。

## 思考
---
## 常见问题
---
## 相关阅读  
---