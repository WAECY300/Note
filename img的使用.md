该文件是以.md格式结尾的文件

"##"属于二级标题

"###"3级标题

。。。。。

"######"六级标题

----

```python
print(233)
```



## img的使用

我是对img标签的介绍

使用"----"4个分隔线来实现下划线分割的效果

```php+HTML
<img src="" alt="" title="" style=""/>
```

`````javascript

`````

//使用"```" 数字1旁边的波浪号，按三次，然后选择语言（php -java -python -c -html -js -MySQL）敲击回车

----

+ ```java
  System.out.print("输出终端内容！！！")
  ```

### 使用方式

使用">"来制作下面的效果

+ "+"可以用来制作列表项

+  按*`tab`*可以把1级列表变成2级列表

+ 从上一行按回车键后，继续按tab可以生成三级列表

  

  + ```
    <background-image:url();>
    ```

  + 在上一行按回车键，进入到当前行后，继续按回车键，可以从当前列表生成上一级列表

  + ```
    
    ```

  + 

  + 在下级列表时可以多次通过按回车键回到一级列表
  + markdown
  + 正常情况下，加号"+"是**无序列表** "-"**是有序列表**

----





> <img src="" alt="" title="" width="" style=""

>我是标注

![拳皇，不只是格斗！](IMG\0.jpg)

![。。。。。。。。](\IMG\0.jpg)

[菜鸟教程:html](https://www.runoob.com/)



连接形式的文本  快捷键ctrl+k  [文字](菜鸟教程)

| ----序号---- | ----姓名----- | ----年龄---- | ----身高---- |      |      |
| :----------: | ------------- | ------------ | ------------ | ---- | ---- |
|              |               |              |              |      |      |
|              |               |              |              |      |      |
|              |               |              |              |      |      |

| ---- | ---- | ---- | ---- |
| :--: | :--: | :--: | :--: |
|      |      |      |      |

[O(∩_∩)O哈哈~](https://www.runoob.com/)

# a标记

> <a href="">超级链接标签</a>

​		a标签在html中用于网页与网页之间的跳转，或者是网页内部的跳转。对于a标签我们的使用有2种方式

## 1.网页与网页之间的跳转

+ 跳转形式有2种
  + 1.绝对路径
    + 固定域名的网络地址，都可以称之为绝对路径
    + https://www.baidu.com
  + 2.相对路径
    + 从当前文件的位置，访问指定位置的html文件
    + ./../../xxx.html
    + ![1600329571399](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1600329571399.png)
    + 在20-917文件夹下，存有2个文件a.html和a-1.html

![1600329935360](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1600329935360.png)

----

+ a.html ![1600330241858](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1600330241858.png)
+ a-1.html![1600330275863](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1600330275863.png)

+ ![1600332629433](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1600332629433.png)
+ ![1600332649678](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1600332649678.png)
+ 以上俩个页面可以互相跳转



----

## 2.a标签的锚标记方法使用

+ a的锚标记方法是可以用href属性定位其他元素的name属性，通过连接查找name值，进行同页面跳转。在href属性中，#代表查找的意思
+ 通过href属性查找指定的name名字。实现锚标记跳转效果。
+ 此处有图，请看下方文字自行想象~~~
+ 注意：当我们p的内容距离小。所以需要在p与p之前用br来撑开距离
+ 通过用a的name属性来定义锚标记点。在用href属性查找

----

+ 通过定义和查找。即可实现同页面锚标记跳转
+ 查看效果:取代码。自己去测试。

