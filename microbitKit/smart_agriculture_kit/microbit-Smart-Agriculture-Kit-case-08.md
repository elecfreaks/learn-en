# 自动采摘装置


##  简介
---
 
- 在坚果类水果采摘过程中，多采用竹竿或木杆等杆体对果树树枝直接击打使成熟果实掉落，再拾取。然而该种方式对树枝和树叶的损伤较大，容易造成后续年头产量减产的问题。所以我们可以制作一个自动采摘装置，通过摇晃树干使果实掉落。

##  功能
---
- 通过舵机摇晃树枝，使果实掉落。

## 购买链接
---
- 1 x [microbit Smart Agriculture Kit]()

## 产品图片
---
![](./images/microbit-Smart-Agriculture-Kit-case-01-02.png)

## 硬件链接
---

将舵机连接到IOT:bit的P1端口。

![](./images/microbit-Smart-Agriculture-Kit-case-08-03.png)

## 软件编程
---
在MakeCode的代码抽屉中点击“高级”，查看更多代码选项。

![](./images/microbit-Smart-Agriculture-Kit-case-01-04.png)

为了给舵机编程，我们需要添加一个扩展库。在代码抽屉底部找到“扩展”，并点击它。这时会弹出一个对话框，搜索”servo“，然后点击下载这个代码库。

![](./images/microbit-Smart-Agriculture-Kit-case-01-06.png)


*注意：*如果你得到一个提示说一些代码库因为不兼容的原因将被删除，你可以根据提示继续操作，或者在项目菜单栏里面新建一个项目。

## 程序
---

设置舵机转动到90度，延迟200ms，然后转动到0度，在延迟200ms。

![](./images/microbit-Smart-Agriculture-Kit-case-08-07.png)



请参考程序连接：[https://makecode.microbit.org/_EdPD6HckVEuE](https://makecode.microbit.org/_EdPD6HckVEuE)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_EdPD6HckVEuE" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  


## 结果
---
- 通过舵机摇晃果树，使果实掉落。



