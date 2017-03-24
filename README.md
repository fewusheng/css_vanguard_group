>    # CSS先锋小组
>     CSS_vanguard_group
>                
> ####  前端CSS先锋小组，成立于2017年3月15日。
>
>     本群专做CSS技术的学习和讨论，
>
>      欢迎广大的朋友进来分享自己学习的心得，
>
>      小组定期发布关于CSS的一些任务，
>
>     具体的规则请加入CSS小组查看，
>
>      本人也不喜欢绕圈子，
>
>     我希望大家在CSS先锋小组获得自己的成绩！
>
>     我也希望大家能在小组的生活中相处的愉快！
>     
>      
>![image](http://mmbiz.qpic.cn/mmbiz_png/XDRSSguXlR4I0vO2ATzoNItYib7cibuaeicfc6iapXicSMWpDzjX6DyoDxUvicEzy5ktembrJajRYuRC42YuSbOIpOFw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)
---
>[CSS先锋计划](https://mp.weixin.qq.com/s?__biz=MzI4ODA1MTMwOQ==&mid=2247483688&idx=1&sn=2af4588d4cffc50f4c7f4a0f2f7713d3&chksm=ebc5182adcb2913cb3e849fbafadd2f4944682b46d0fc3b555cfd812ece6f01efe9f54b241ae#rd)

---

### 2017.03.16

***第一次任务***
---
>#  [Task1](http://mp.weixin.qq.com/s/-fulS8uVqkhQ-SUKTu6yPQ)
---
>##  已经提交作业者
ID | 评价   |   ID | 评价
---|---     |---|---
雪梅 | 良   |无笙 | 优
王艳丹 | 良   |我吃包才菜 | 良
差不多先生|良  |风继续吹 | 良
Chris|良      | 明道若昧 | 良
🐝🐝|优      | 小丽子 | 良
Mark|优       | ______荒城旧梦 | 良 
>
---
>
>[代码](https://github.com/Mao605569464/task01)
---

  *本次我们的要求不需要任何其它样式，我看到还是有很多朋友没有按照规则分开写样式。不过没关系，希望大家下次按照要求写*
  #### 关于（内联，外部，外链样式）
  >这三种样式是有优先级的，
  >记住他们的优先级：内联式>嵌入式外部式，
  >但是嵌入式>外部式有一个前提：
  >嵌入式css样式的位置一定在外部式的后面。
  >其实总结来说，就是--就近原则（离被设置元素
  >越近优先级别越高）。
  >但注意上面所总结的优先级是有一个前提： >内联式、嵌入式、外部式样式表中css样式是在的>相同权值的情况下。
  ##### 内联样式的优缺点
  ##### 优点：
  >内联样式表比较灵活，
  >可单独制定某一标签的独特性；
  >
  ##### 缺点：
  >效率不够高，代码不易整理，
  >不能同时改变多个标签的属性。
  >
  >而与内联样式相反的就是，
  >调入外部css样式表。
  >将规则写入一个单独的样式表文件中，
  >然后使用href="*.css"
  >将整个样式表文件导入到页面就行了。
  >
  ### 2017.03.23
**第二次任务**
---
>#  [Task2](http://mp.weixin.qq.com/s/GqBV_gBSOaFEX7PCUYABHQ)
>#  [Task3](http://mp.weixin.qq.com/s/8danlGk0dExPXxSWkTCGxg)
>#### [附CSS定位视频](https://v.qq.com/x/page/m03862mf3y.html)   
---


>#####  绝对定位
>如果想为元素设置层模型中的绝对定位，
>需要设置position:absolute(表示绝对定位，
>这条语句的作用将元素从文档流中拖出来，
>然后使用left、right、top、bottom属性>
>相对于其最接近的一个具有定位属性的父包含>块进行绝对定位。
>如果不存在这样的包含块，
> 则相对于body元素，即相对于浏览器窗口，
>而其层叠顺序则通过z-index属性来定义。
>如下面代码可以实现div元素相对于浏览器窗>>口向右移动100px，向下移动50px。
```
<html>
<head>
<style type="text/css">
div{
    width:200px;
    height:200px;
    border:2px red solid;
    position:absolute;
    left:100px;
    top:50px;
}
</style>
</head>
<body>
    <div id="div1"></div>
</body>
</html>
```
>###  代码实现如下
![image2](http://mmbiz.qpic.cn/mmbiz_png/XDRSSguXlR5WQibpywhh9ejwIWI9V9YK5MbJcIavSTgKWTFkM1CriaVTuL4BJOliaRzbRpmlYTeZvwibwxCwvrASmQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)
>#####  相对定位
>如果想为元素设置层模型中的相对定位，
>需要设置position:relative
>（表示相对定位），
>它通过left、right、top、bottom属性
>确定元素在正常文档流中的偏移位置。
>相对定位完成的过程是首先按static(float)
>方式生成一个元素，
>相对于以前的位置，移动方向和幅度
>由left、right、top、bottom属性确定，
>偏移前的位置保留不动。
>如下代码实现相对于以前位置向下移动20px，>向右移动100px;

```
<html>
<head>
<style type="text/css">
#div1{
    width:200px;
    height:200px;
    border:2px red solid;
    position:relative;
    left:100px;
    top:50px;
}
</style>
</head>
<body>
<div id="div1"></div>
</body>
</html>
```

>###   代码实现如下：
>![image](http://mmbiz.qpic.cn/mmbiz_png/XDRSSguXlR5WQibpywhh9ejwIWI9V9YK5OX3gM9fOMfiaJOGics0k0U7yNOa48DIlEHIs37nSG4l40sf2pdx0ApDA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)

>#####  固定定位
>fixed：表示固定定位，与absolute定位类型类似，
>但它的相对移动的坐标是视图（屏幕内的网页窗口）本身。
>由于视图本身是固定的，
>它不会随浏览器窗口的滚动条滚动而变化，
>除非你在屏幕中移动浏览器窗口的屏幕位置，
>或改变浏览器窗口的显示大小，
>因此固定定位的元素会始终位于浏览器窗口内视图的某个位置，
>不会受文档流动影响，这与background-attachment:fixed;
>属性功能相同。以下代码可以实现相对于浏览器视图向右移动100px，
>向下移动50px。并且拖动滚动条时位置固定不变。

```
<html>
<head>
<style type="text/css">
div{
    width:200px;
    height:200px;
    border:2px red solid;
    position:fixed;
    left:500px;
    top:50px;
    font-size:30px;
    font-weight:bold;
    text-align:center;
    line-height:200px;
}
</style>
</head>
<body>
<div>CSS先锋小组</div>
<p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p><p>文本</p>
</body>
</html>   
```
>实际效果需要滑动浏览器的滚动条才能看到，>所以就不演示了。大家请拷贝以上代码自行测试，
    **注意**：P标签尽量要多些,才能显示滚动条。
    **注意**：IE浏览器对固定定位支持不理想


