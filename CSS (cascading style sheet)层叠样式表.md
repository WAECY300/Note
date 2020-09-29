CSS (cascading style sheet)层叠样式表

用于修饰html标记语言的样式。可以改变颜色。宽高。大小。形状。位置等

css的使用有三种不同的方式

内联--外联--内部

`内联`：在head中书写的style标签，在标签内书写的样式，称为内联标签   权重 10

`外联`：通过在head中书写link标签，再通过href连接外部css样式表   权重 10

`内部`：在标签上书写的style属性  权重1000



# CSS的基本样式

### 针对于文本的修饰

+ 文本颜色	

  + color：颜色
    + 英文
      + red         #ff0000
      + blue       #0000ff
      + black     #000000
      + green    #00ff00
      + pink       
      + gray、grey
      + white
      + yellow
      + .......
    + 16进制码   ps中的颜色  0123456789abcdef
      + #000000 黑色
      + #ffffff  白色
      + #ff0000  红色
      + #00ff00  绿色
      + #0000ff  蓝色
      + #ffff00    黄色
      + #ff00ff     紫色（洋红色）
      + #00ffff     青色  
      + transparent  透明
      + .......
    + rgb(0~255,0~255,0~255)hsb
      
      + rgb(红，绿，蓝)
    + rgba(0~255,0~255,0~1)
      + r 红色 0~255之间的值
      + g 绿色0~255之间的值
      + b 蓝色0~255之间的值
      + a 透明度 0代表透明  1代表不透明
      
      

+ 加粗

  + font-weight:
    + bold 重（加粗）
    + 指定赋值+单位像素（px）eg：300px
    + normal：正常

+ 倾斜

  + font-style:值
    + italic 倾斜
    + normal 正常

+ 下划线

  + decoration：装饰，修饰。。。

  + ```html
    text-decoration:underline;(下划线)
    text-decoration:overline;(上划线)
    text-decoration:line-through;(删除线)
    text-decoration:none;(无)
    ```

+ 字体大小

  + font-size:16px

+ 文本排列

  + text-align：left、center、right
  
+ 行高

  + line-height：20px；
    + 行高是可以撑开元素的高度的

+ 文本阴影

  + text-shadow：水平位置  垂直位置  模糊程度  颜色

  + ```html
    text-shadow:10px 5px 10px black
    ```
    
  + ![1601133267568](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1601133267568.png)

+ 空白处理

  + white-space：值
    + pre  文本域格式化（按照书写格式，显示文本）文本不会换行，超出部分继续显示。页面会出现横向滚动条
    + normal  正常
    + nowrap   不换行
    + pre-wap    一行内超出的部分，会自动换到下一行
  + 文本溢出
    + text-overflow：ellipsis 省略号
  + word-spacing 
    + 文字间距（英文效果最好）
      + 主要针对有空格的语句，正常情况下不针对中文。针对于的对象为英文短句。
  + 首行缩进
    + text-indent:像素

## box盒子模型

指代的是盒子尺寸的属性



## content 内容区

  ### width

min-widrh --最小宽度

max-height  最大高度

### height



### border

### 1 . 四面边框

+ 边框  
+ 大小：
  + 像素
+ 线：
  + solid         实线
  + dashed    虚线
  + dotted      点线
  + double      双线
+ 颜色：
  + 英文 、16进制、rgb、rgba

## 2.单独边框

+ border-left

+ border-top

+ border-bottom

+ border-right

+ 三个元素（color-width-style）【颜色-大小-样式】必须一起出现（不分顺序）

+ 例如：

  + ```html
    border-right:30px red dashed;
    border-top:10px #ffffff solid;
    border-bottom:10px #ff00ff solid;
    border-left:30px #0000ff dashed;
    ```

## 3、边框的属性单独设置

+ 3.1 四面边框单独设置
  + border-color
  + border-width
  + border-style
+ 3.2 单面边框的设置
  + border-left-color
  + border-right-width
  + border-left-style
  + 其余相同

## 4、边框圆角（CSS3）

+ border-radius（半径）：

  + r半径

    + x 水平半径

    + y 垂直半径

    + border-radius:x/y

    + ```
      border-radius:20px/40px;
      ```

      + 这种一般是读取的一个角，都是按照水平垂直来计算的，其余角都相等。

    

    ## 同时设置4个圆角

    >border-radius:r

    该书写形式，同时指定4个角为统一的圆角

    ```
    border-radius:40px;
    //4个角都是40px的圆角
    ```

    >
    >
    >2.border-radius:20px 30px;

    该书写形式，指定左下=右上  右上=左下

    >
    >
    >3.border-radius：20px 40px 60px

    该书写的形式，没有值的角，取对角的圆角值

    即左上角==20px、右上角==左上角==40px、右下角==60px

    >
    >
    >4、border-radius:20px 40px 30px 60px

    分别指代左上-右上-右下-左下

    >
    >
    >5、圆角的水平半径和垂直半径不相同

    border-radius：10px/49px

    水平半径10px   垂直半径49px

    >
    >
    >6、border-radius：rx1 rx2 rx3 rx4/ry1 ry2 ry3 ry4

    rx代表水平半径   ry代表垂直半径

    ```css
    border-radius:10px 20px 30px 40px/5px 8px 11px 30px;
    ```

    

    

    + border-radius:r1 r2;

    + ```
      border-radius:20px 40px
      这个写法，我们发现出现的圆角
      左上角=右下角==20px
      左下角=右上角==40px
      ```

    ## 指定圆角

    + border-top
      + border-top-left-radius
      + border-top-left-radius
    + border-bottom
      + border-bottom-left-radius:x y
      + border-bottom-right-radius:x y

## margin（外边距）

外边距：不存在颜色，可以撑开多个元素之间的距离

在正常情况下，相交的俩个外边距，取最大值

+ ```
  margin:right left top bottom;
  ```

  写法

  

+ margin:10px

  + 代表4个边都有10像素的外边距

+ margin:10px 20px

  + 代表上下有10像素外边距，左右20像素外边距

+ margin：10px 20px 30px

  + 代表`上边10px` `左右20px`  `下30px`

+ margin：10px 20px 30px 40px

  + 分别代表上 右   下    左

+ 某个方向有外边距

  + margin-left
  + margin-right
  + margin-top
  + margin-bottom
  
  ## 2、margin做盒子居中
  
  margin可以让有宽度的块级元素相对于它的父元素做水平居中设置
  
  ```html
  单独书写:margin-left：auto；margin-right：auto；
  整合书写:margin:0 auto;
  ```
  
  margin不能改变元素上下居中的设置，只能通过自己计算值来设置margin值

# 五、padding（内填充）

内填充，作用在border以内，width和height以外

padding所占据的位置不能提供给内容（文本、图片、其他盒子等）元素使用

padding的使用方式与margin相同。详细看margin



盒模型有哪几个

​     width  height     padding    border   margin

​	background：

​		background-image：url



## 浮动

float

在默认的文档布局中，通常情况下，块级元素是不能在同一行显示的。如果我们希望块元素在一行内显示多个，需要让元素处于脱离文档流的一个状态。

​		在正常页面的书写中，我们发现标签是流式向下顺序排列的（默认文档流）

```
float: left/right
```

+ 浮动

  + left 左侧
  + right 右侧

+ 注意：

  + 浮动的元素会影响其他元素的位置排列

+ 需要处理这个问题：如何解决浮动后的元素对其他元素的影响

  》》》解决对同级元素的影响》》》》》》》》》》》》

  + 1、为浮动的元素添加一个父元素，给父元素设置一个高度
    + 死板--当子元素的位置改变，父元素还要调整高度等问题
  + 2、为浮动元素添加一个父元素，为父元素设置overflow：hidden
    + 注意：不需要为父元素设置高度
  + 3、为浮动元素紧挨着的下一个元素添加clear属性
    + clear：left、right、both
      + both（俩边同时）
    + clear可以清除浮动元素的影响

  2、对于父元素的影响

  浮动的元素，脱离文档流后，会影响其父元素的高度

  解决：

  + 上述为父元素的设置，可以解决这个问题

  + 在父元素的所有子元素最后边添加一个空的div元素（无内容-无高度），对于该div元素，设置clear：both样式，即可解决

  + 对浮动元素的父元素，使用伪类样式，解决问题

    ```html
    .d2::after{
    												content:"我是伪类元素";
    												display:block;
    												float:both;
    
    		border: 10px dashed gold;
    
    		font-weight:bold;
    
    		  }
    ```

    



CSS伪类



display



opacity



组合选择符（空格和，）



CSS属性选择器



轮廓   ---none



扁平化 - 设计



### 其他属性

# 一 .background

### 1、background-color

​	值与color的颜色值用法一致

### 2、background-image

​		![1601132674695](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1601132674695.png)

>background-image:url("路径"); 规范类写法

   		线性渐变（Linear Gradients）

​		   径向渐变（Radial Gradients）

+ ### url	

  + 统一资源定位器
    + 包含有src url href
  + 绝对路径
    + http://sihfaodefiefofjesif.gif
    + https://300jump.com
  + 相对路径
    + 当前文件夹下有images文件夹，文件夹有图片
      + url(./images/xx.jpg)
    + 当前文件路径中直接存有某张图片
      + url(./xx.jpg)

### 3、background-repeat

>
>
>background-repeat:
>
>repeat      
>
>no repeat
>
>repeat-x
>
>repeat-y

+ repeat
  + 重复、平铺（默认值）
+ no-repeat
  + 不重复
+ repeat-x
  + 水平重复
+ repeat-y
  + 垂直重复

### 4、background-position

​	用于调整背景图片的位置。形状的左上角默认为原点（0，0）以原点位置为基准，形状内为正值，形状外为负



![img](file:///d:\Documents\Tencent Files\1412973458\Image\Group2\2F\I`\2FI`4TI66KB$QQOY21EK[6R.png)

+ 值的使用方式
  + 数值
    + x和y可以按照数值的形式书写，单位为px
  + 位置
    + left
    + right
    + center
    + top
    + bottom
    + 通过位置值，我们可以确定固定的9个点
      + 1、left top
      + 2、left center
      + 3、left bottom
      + 4、top center 、center top
      + 5、center   简写  全写（center center）
      + 6、center bottom
      + 7、right top
      + 8、right center
      + 9、right bottom
  + 数值+位置
    + 一般用于在固定的边上，距离某一个边有一定的值

### 5、background-size

+ 值的使用方式
  + 数值
  + cover  等比例缩放
    + 图片的宽度=形状的宽度（div的宽度）
    + 图片的高度=图片宽度的比例值
    + 例如：图片大小为100 * 30，div盒子的大小为500 * 100，如果背景图的大小值设置为cover后。首先图片宽度从100提升到500，也就是宽度提升5倍，那么图片的高度也将放大5倍。从30提升到50
  + 百分比
    + background-size:100% 100%
    + 图片的宽度=盒子的宽度
    + 图片的高度=盒子的高度

### background的整合写法：

``` 
background:color url() repeat position
```



### background-origin属性

![1601132315304](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1601132315304.png)

![1601132355252](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1601132355252.png)

## class 类

定义class类用于对页面中相同的元素，设置不同的效果

>
>
>注意：在定义class类的时候，不允许数字开头

​       例如：

		## 标题

```html
   <h1 class="2a">标题</h1>
```

这个写法是错误的，浏览器不能解析当前的class类，也就不能对类属性进行赋值



## 使用



class定义的类名称，在style样式书写时，需要添加“.”用于识别类名

例如:

```
<style>
       .a1{
            font-size:20px;
            font-weight:normal;
          }
</style>
```

## id

对于html元素设置id属性，同一页面中不允许出现重复的id名字

代码在执行的过程中，虽然会使用就近原则（离html越近的样式，执行力越高），但是id的默认权重值为100，class类名的权重只有10，所以class的样式修改不成功

## 权重

类名称+css的使用方式来判断css样式的权重级别

> 内部的样式读取级别大于其他俩种方式的引入

>注意: <sapn style="color:gold"><b>权重</b></span>还有累加性

