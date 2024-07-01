# day01-2.14

## 1.认识网页

网页组成部分：文字，图片，音频，视频，超链接；

五大浏览器：

•        IE浏览器

•      火狐浏览器(Firefox)

•      谷歌浏览器(Chrome)  推荐使用

•       苹果Safari浏览器

•      欧朋浏览器(Opera)

transform: translate() ;
处理谷歌苹果浏览器兼容-webkit-transform: 
处理火狐浏览器兼容-moz-transform:
处理欧朋浏览器兼容-o-transform: 
*处理iie浏览器兼容*/-ms-transform: ;

## 2.web标准

•     结构： HTML → 页面元素

•     表现：  CSS → 页面样式

•     行为：  JavaScript → 页面交互的动态效果

## 3.html骨架结构

•     html标签：网页的整体(外围主体)

•     head标签：网页的头部

•     body标签：网页的身体

•     title标签：网页的标题

## 4.常用的快捷键

•     快速生成结构标签：  ! + tab或者回车

•     快速查看网页效果：alt+b

•     快速复制一整行： ctrl + c

•     快速粘贴一整行： ctrl + c+v

•     快速删除(剪切)一整行：  ctrl + x

•     注释：ctrl+/

alt + ↑ / ↓  批量移动代码段
alt + shift + ↑ / ↓  批量复制代码段

shift + home  将光标切换到行首

shift + end  将光标切换到行尾
ctrl + enter  从当前位置切换到下一行

​	<!-- !红色 -->

​        <!-- ?蓝色 -->

​        <!-- //删除线 -->

​        <!-- todo橙色 -->

​        <!-- *浅绿色 -->

•     选中下一个相同文本：ctrl+d

## 5.标签关系

•      父子关系(嵌套关系)

•      兄弟关系(并列关系)

## 6.标题标签

<h1>我是一级标题<h1>

➢ 特点：

•   只有6级，重要程度依次递减

•      文字都有加粗

•      文字都有变大，并且从h1→ h6文字逐渐减小

•      独占一行

## 7.段落标签

<p>我是一段文字</p>

➢  特点：

•      段落之间存在间隙

•      独占一行

•      p标签不能嵌套p标签和h系列标签

## 8.文本格式化标签

br标签：  单标签     文本的强制换行

 hr标签： 独占一行  单标签   显示一条分割线

​    <b>加粗标签</b>

​    <strong>具有强调意义的加粗标签</strong>

​   <u>下划线标签<u>

​    <ins>具有强调意义的下划线标签</ins>

​    <i>我是一个倾斜标签</i>

​    <em>具有强调意义的倾斜标签</em>

​    <s>删除线标签</s>

​    <del>具有强调意义的删除下线标签</del>

## 9.图片标签

```html
<img src="猫咪.jpg" width="540" height=""  alt="404 not found" title="这是一只可爱的猫咪">
```

•     src 	目标图片的路径

•     width height	只设置其中一个时，另一个等比缩放

•     alt	替换文本 当图片加载失败时，才显示alt的文本（路径错误 网络问题）

•     title	提示文本 当鼠标悬停时，才显示的文本（文本不宜过多）

## 10.音频标签

```html
<audio src="./music.mp3" controls loop></audio> 
```

•     src	音频路径

•     controls	显示播放的控件

•     loop	循环播放

•     autoplay	自动播放（音频不支持）

## 11.视频标签

```html
 <video src="./video.mp4" controls loop  autoplay muted></video>
```

•     支持自动播放但需搭配muted使用

•     有长宽设置(写在style标签内)

## 12.超链接

```html
<a href="./day1-9下级目录/day1-10难度提升/day1-11路径.html" target="_blank">跳转</a>
    <a href="#" target="_self">跳转</a>
```

•     href	链接路径

•     target 	_self默认，覆盖原网页；

​			_blank在新窗口跳转，保留原网页；

•     #	空链接，点击之后回到网页顶部；

➢  特点：

•      双标签，内部可以包裹内容

•      如果需要a标签点击之后去指定页面，  需要设置a标签的href属性

➢  显示特点：

•      a标签默认文字有下划线

•      a标签从未点击过，默认文字显示蓝色

•      a标签点击过之后，文字显示为紫色

## 13.路径

➢  绝对路径：指目录下的绝对位置，可直接到达目标位置，通常从盘符开始的路径

•   例如：盘符开头：  D:\day01\images\1.jpg

➢  相对路径：从当前文件开始出发找目标文件的过程

➢  相对路径分类：

•      同级目录

•      下级目录

•      上级目录

# day02-2.15

## 1.无序列表  ul

```html
 ul>li*5
 ul>li{$}*5
<ul type="circle"> 
        <h1>一级标题</h1>
        <li>2斤猪肉</li>
        <li>10箱啤酒</li>
        <li>3斤可乐</li>
    </ul>
```

➢特点：	•   自带黑色小圆点

​		•   排列方式整齐

​		•   独占一行

➢type类型：disc 默认黑色实心圆点；circle 空心圆；square 黑色实心方块；none 取消列表项；

## 2.有序列表 ol

```html
<ol type="A" start="2">
        <h1>手机销量排行</h1>
        <li>
            <em>华为手机</em>
        </li>
        <li>小米手机</li>
        <li>oppo手机</li>
        <li>vivo手机</li>
    </ol>
```

•    type(类型) = "A/a/I/i/1"

•   stare    从第几位开始排列

## 3.自定义列表

•    dl标签：表示自定义列表的整体

•    dt标签：表示自定义列表的主题

•    dd标签：表示对于主题的每一项内容	自带首行缩进效果

注：dl标签中只允许包含dt/dd标签，dt/dd标签可以包含任意内容，dd不能包含dt

```html
 <dl>
        <h1>一级标题</h1>
        <dt>我的</dt>
        <dd>收货地址</dd>
        <dd>全部订单</dd>
     </dl>
```

## 4.表格 table

```html
<table border="1" width="100" height="100">
        <caption> <strong>成绩单</strong></caption>
        <tr>
            <th>1</th>
            <th>2</th>
            <th>3</th>
        </tr>
        <tr>
            <td>1</td>
            <td>2</td>
            <td>3</td>
        </tr>
    </table>
```

•  标签的嵌套关系：table >tr> td

•    table	表格整体，用于包裹多个tr

•    tr	表格每行，用于包裹td

•    td	表格单元格，包裹内容

•    表格相关属性	：	border 边框宽度；width 表格宽度；height 表格高度；（数字）

​				caption 表格大标题  表示表格整体大标题，默认顶部居中

​				th 表头单元格 替换td表示一列小标题，默认内部文字加粗居中

## 5.表格结构

•   thead：表格头部

•   tbody：表格主体

•   tfoot：表格底部

注：表格结构标签写在table标签内部，表格标签内部用于包裹tr标签

```html
<table border="1" height="500" width="500">
        <thead>
            <tr>
                <td>1</td>
                <td>2</td>
                <td>3</td>
            </tr>
        </thead>
        <tbody height="50">
            <tr>
                <td>1</td>
                <td>2</td>
                <td>3</td>
            </tr>
            <tr>
                <td>1</td>
                <td>2</td>
                <td>3</td>
            </tr>
            <tr>
                <td>1</td>
                <td>2</td>
                <td>3</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <td>1</td>
                <td>1</td>
                <td>1</td>
            </tr>
        </tfoot>
    </table>
```

## 6.单元格合并

•    rowspan：上下 跨行合并→垂直方向合并

 •    colspan：左右 跨列合并→水平方向合并

通过左上原则，确定保留谁删除谁

```html
<table border="10" width="300"  height="300">
        <tr>
            <td rowspan="2">1</td>
            <td>2</td>
            <td rowspan="2" colspan="2">3</td>
            <!-- <td>4</td> -->
        </tr>
        <tr>
            <!-- <td>1</td> -->
            <td>2</td>
            <!-- <td>3</td> -->
            <!-- <td>4</td> -->
        </tr>
        <tr>
            <td>5</td>
            <td>6</td>
            <td colspan="2">7</td>
            <!-- <td>4</td> -->
        </tr>
        <tr>
            <td>9</td>
            <td>10</td>
            <td>11</td>
            <td>12</td>
        </tr>
    </table>
```

## 7.input系列标签

改变placeholder样式：

&::-webkit-input-placeholder{

​                    color: #3C3C3C ;

​                }

```html
<form action="../day-1/day1-9下级目录/图片.jpeg" target="_blank">
        <h1>欢迎光临</h1>
            <!-- text 文本框 -->
        账号：<input type="text" placeholder="请输入账号">
        <br> <br>
            <!-- password 密码框  placeholder 占位符-->
        密码：<input type="password" placeholder="请输入密码">
        <br>
        <br>
            <!-- radio 单选框 name  , 同一组只能单选 checked 默认选择 -->
        <input type="radio" name="one" checked>公
        <input type="radio" name="one">母
        <br>
        <br>            
  			<!-- 没必要加name ,可以加checked , checkbox复选框 -->
        爱好：<input type="checkbox">唱<input type="checkbox" checked>跳<input type="checkbox">篮球
            <!-- file 文件选择 , mutiple 多选文件 -->
        <input type="file" multiple>
        <br>
        <br>
            <!-- submit 提交 , reset 重置 , button 普通按钮 -->
        <input type="submit" value="登录">
        <input type="reset" value="清除">
        <input type="button"  value="普通按钮">
    </form>
```

## 8.button按钮标签

```html
 <!-- 如果没有类型限制，默认是提交按钮 -->
    <button>按钮</button>
    <button type="submit">提交</button>
    <button type="reset">重置</button>
    <button type="button">普通</button>
```

•    type属性：submit  提交按钮，点击后提交数据到后端服务器；reset  重置按钮

## 9.下拉菜单 select

```html
<select name="" id="">
        <option value="" selected>武汉</option>
        <option value="">北京</option>
        <option value="">上海</option>
    </select>
```

•    select 下拉菜单的整体;   option 菜单中的一项 ; selected  默认选项;

## 10.文本域  textarea

```html
<textarea name="" id="" cols="4" rows="3"></textarea>
    <textarea name="" id="" cols="6" rows="10"></textarea>
```

•    cols 文本框宽度；row 文本框高度；（数字）

## 11.label标签

```html
<input type="radio" name="one" id="A"><label for="A">男</label> 
    <input type="radio" name="one" id="b"><label for="b">女</label> 

    <label >
        <input type="radio" name="c">男
    </label>
    <label>
        <input type="radio" name="c">女
    </label>
```

使用方法①：

​	使用label标签把内容（如：文本）包裹起来，在表单标签上添加id属性，在label标签的for属性中设置对应的id属性值。

使用方法②：

​	直接使用label标签把内容（如：文本）和表单标签一起包裹起来，需要把label标签的for属性删除即可。

## 12.语义化标签

```html
	<div>独占一行标签</div>
    <header>网页头部</header>
    <footer>网页底部</footer>
    <nav>网页导航</nav>
    <article>网页文章</article>
    <span>1</span>
    <span>2</span>
```

•    标签显示特点与div一致，多了不同的语义

## 13.字符字体

| 显示结果 |  描述  |  实体名称  |
| :--: | :--: | :----: |
|      |  空格  | ￥nbsp; |
|  <   |      |        |
|  >   |      |        |
|  &   |      |        |
|  “   |      |        |
|  "   |      |        |
|      |      |        |
|      |      |        |
|      |      |        |
|      |      |        |
|      |      |        |
|      |      |        |

![图片1](C:\Users\86159\Pictures\图片1.png)

# day03-2.16

## 1.css（层叠样式表）语法

•    css写在style标签中，style标签一般写在head标签里面，title标签下面

```html
 <style>
        p{
            /* 文字颜色 */
            color: green;
            /* 字体大小 */
            font-size: 30px;
            /* 背景颜色 */
            background-color: greenyellow;
            /* 宽度 */
            width: 300px;
            /* 高度 */
            height: 200px;
        }
        span{
            background-color: red;
            /* width不管用 */
        }
        div{
            /*  缩写w300+h300+bgc
            width: 300px;
            height: 300px;
            background-color: #fff; */
            width: 300px;
            height: 300px;
            background-color: green;
        }
```

## 2.css的引入方式

➢内嵌式：CSS 写在style标签中

•    提示：style标签虽然可以写在页面任意位置，但是通常约定写在head 标签中

```html
<style>
        div{
            color: red;
        }
    </style>
```

➢外联式：CSS 写在一个单独的.css文件中

•    提示：需要通过link标签在网页中引入  rel(当前文件与被链接文件之间的关系)="stylesheet(样式表)"

不用再写style标签

```html
<link rel="stylesheet" href="./2css外联.css">
```

```html
<style>
        @import url(./4css外联2.css);
    </style>
```

link和import之间的区别？

①  差别1：本质的差别：link属于XH

②  TML标签，而@import完全是CSS提供的一种方式。 

③  差别2：加载顺序的差别：当一个页面被加载的时候（就是被浏览者浏览的时候），link引用的CSS会同时被加载，而@import引用的CSS会等到页面全部被下载完再被加载。所以有时候浏览@import加载CSS的页面时开始会没有样式（就是闪烁），网速慢的时候还挺明显。

④  差别3：兼容性的差别：@import是CSS2.1提出的，所以老的浏览器不支持，@import只有在IE5以上的才能识别，而link标签无此问题。

⑤  差别4：使用dom(document o bject model文档对象模型 )控制样式时的差别：当使用javascript控制dom去改变样式的时候，只能使用link标签，因为@import不是dom可以控制的.

➢行内式：CSS 写在标签的style属性中

•    提示：基础班不推荐使用，之后会配合js使用

```html
<div style="font-size: 50px;">
        div标签
    </div>
```

•    优先级： 行内式优先级高于内嵌式和外联式

​        	看标签位置谁距离近显示谁（就近原则）

​        	代码执行顺序（后来者居上）

 •    权重

​            行内式1000

​            内嵌式0001

​            外联式0001

## 3.标签选择器

•   通过标签名，找到页面中所有这类标签，设置样式

•   标签选择器选择的是一类标签，而不是单独某一个

•   标签选择器无论嵌套关系有多深，都能找到对应的标签

## 4.类选择器

•  类选择器以. 开头

•   类名可以由数字、字母、下划线、中划线组成，但不能以数字或者中划线开头

 •   一个标签可以同时有多个类名，类名之间以空格隔开

•   类名可以重复，一个类选择器可以同时选中多个标签

```html
 <style>
        .color{
            color: red;
        }
        .size{
            font-size: 50px;
        }
    </style>
</head>
<body>
    <div class="color size">
		我是一个div标签
    </div>
    <p class="color">
        我是一个p标签
    </p>
</body>
```

## 5.id选择器

•   id选择器以\# 开头

•   所有标签上都有id属性

•   id属性值类似于身份证号码，在一个页面中是唯一的，不可重复的！

•   一个标签上只能有一个id属性值

•   一个id选择器只能选中一个标签

```html
 <style>
        #btn{
            background-color: gold;
        }
        .btn{
            background-color: red;
        }
        #bon{
            background-color: aqua;
        }

    </style>
</head>
<body>
    <button type="submit" id="btn">提交</button>
    <button class="btn" id="bon">按钮</button>
</body>
```

## 6.通配符选择器 *

•   找到页面中所有的标签，设置样式

```html
*{
            /* 外边距 */
            margin: 0;
            /* 内边距 */
            padding: 0;
        }
取消页面边距
```

➢通用兄弟选择器  h1+p~p  两个p及后面的都选中

➢相邻兄弟选择器  h1+p  p选中

## 7.字体和文本样式 font

➢字体大小：font-size

•      谷歌浏览器默认文字大小是16px 最小12px

•      单位需要设置，否则无效  数字+px

```html
div{
font-size: 20px;
}
```

➢字体粗细：font-weight

正常 normal;	加粗 bold

纯数字100-900的整百数		正常 400;	加粗 700

```html
<style>
div{
	font-weight:normal;
	font-weight: bold;
	font-weight:bolder;
	font-weight: 600;
}
  </style>
```

➢字体样式：font-style

•      正常（默认值）：normal

•      倾斜：italic（em/i标签实现倾斜）

```html
<style>
  div{
    font-style:normal;
    font-style:italic;
  }
  em{
            font-style: normal;
        }
</style>
```

➢ 字体类型：font-family

•  **无衬线字体**（sans-serif）

•  **衬线字体**（serif）

•  **等宽字体**（monospace）

```html
<style>
.box{
     font-family: "桦源黑体","宋体",sans-serif;
        }
  <style>
```

## 8.font连写

```html
<style>
        div{
            font: italic 700 30px "桦源黑体";
            background-color: beige;
            width: 600px;
            /* 后者需放在连写后面，不然会被覆盖掉 */
        }
    </style>
```

## 9.首行缩进 text-indent:;

1em等于当前标签字体大小。

```html
<style>
        .box{
            width: 800px;
            height: 100px;
            background-color: aquamarine;
            font-size: 15px;
            /* 相对单位 参照当前标签字体大小 */
            text-indent: 2em;
        }
    </style>
```

## 10.水平对齐方式 text-align: ;

```html
<style>
        .box{
            width: 500px;
            height: 400px;
            background-color: aqua;
            /* 居中对齐 */
            text-align: center;
            /* 左对齐 */
            /* text-align: left; */
            /* 右对齐 */
            /* text-align:right; */
        }
  <style>
```

## 11.文本修饰 text-decoration：;

网页精准布局时，会设置 line-height : 1 可以取消上下间距

```html
<style>
        p{
            /* 下划线 */
            text-decoration: underline;
            /* 删除线 */
            text-decoration: line-through;
            /* 上划线 */
            text-decoration: overline;
            /* 无装饰线 */
            text-decoration: none;
           /* 单行文本垂直居中设置行高为文本高度 */
          	line-height:400px ;
        }
```

## 12.颜色取值

rgba表示法:	a的取值范围：0~1

​			1：完全不透明

​			0：完全透明

十六进制表示法:	两个数字为一组，每个数字的取值范围：0~9,a,b,c,d,e,f

​				如果三组中，每组数字都相同，此时可以每组可以省略只写一个数字

![图片2](C:\Users\86159\Pictures\图片2.png)

```html
<style>
        div{
            /* 红绿蓝三原色 */
            background-color: rgb(10, 5, 100);
            background-color: rgba(53, 200, 53, 0);
            /* 十六进制 */
            background-color: #fffaac;
        }
    </style>
```

# day04-2.17

## 1.标签水平居中 margin: 0 auto

如果需要让div、p、h（大盒子）水平居中，直接给当前元素本身 设置即可

margin：0auto一般针对于固定宽度的盒子，如果大盒子没有设置宽度，此时会默认占满父元素的宽度

```html
<style>
        div{
            width: 300px;
            height:300px ;
            background-color: aqua;
            margin: 0 auto;
        }
        p{
            width: 50px;
            height: 50px;
            background-color: #fff;
            margin: 0 auto;
        }
        span{
            display: block;
            width: 100px;
            height:30px ;
            background-color: aqua;
            margin: 0 auto;
        }
    </style>
```

## 2.后代选择器 空格

选择器语法：  选择器1 选择器2 { css }

在选择器1所找到标签的后代(儿子、孙子、重孙子 … )中， 找到满足选择器2的标签，  设置样式

```html
<style>
        /* div p{
            color: red;
        } */
        /* .box p{
            color: aqua;
        } */
        .box div p{
            color: blue;
        }
    </style>
</head>
<body>
    <div class="box">
        div标签
        <p>p标签</p>
        <div>
            我是div2 
            <p>p标签2</p>
        </div>
    </div>
</body>
```

## 3.子代选择器 >

代只包括：儿子

可以和其他选择器搭配使用

子代选择器中，选择器与选择器之前通过 > 隔开

```html
<style>
div p>span{
            color: aqua;
        }
    </style>
```

## 4.并集选择器 ，

作用：同时选择多组标签，设置相同的样式

➢  选择器语法：  选择器1 ，  选择器2 { css }

➢  结果：

•      找到 选择器1和 选择器2 选中的标签，设置样式

```html
<style>
        div>strong,span,header,section~p{
            color: aqua;
        }
    </style>
```

## 5.交集选择器   紧挨着

•    作用：选中页面中 同时满足 多个选择器的标签

•    选择器语法：  选择器1选择器2 { css }

```html
<style>
        div.box{
            color: antiquewhite;
        }
        p#one{
            background-color: aquamarine;
        }
        .box.three#four>span{
            color: blue;
        }
    </style>
```

## 6.hover为类选择器 	标签:hover

•    作用：选中鼠标悬停在元素上的状态，设置样式

```html
<style>
div>p>span:hover{
            color: antiquewhite;
        }
        <style>
```

## 7.emmet语法

•    通过简写语法，快速生成代码

```html
<!-- p.box -->
    <div class="box"></div>
    <!-- span#bob -->
    <span id="bob"></span>
    <!--  -->
    <strong id="tot" class="tob"></strong>
    <!-- ul>li -->
    <ul>
        <li></li>
    </ul>
    <!-- ul>li{$}*3 -->
    <ul>
        <li>1</li>
        <li>2</li>
        <li>3</li>
    </ul>
    <!-- ul*3>li{$}*2 -->
    <ul>
        <li>1</li>
        <li>2</li>
    </ul>
    <ul>
        <li>1</li>
        <li>2</li>
    </ul>
    <ul>
        <li>1</li>
        <li>2</li>
    </ul>
```

## 8.背景图片	background-image

•    背景颜色： background-color:;

```html
<style>
        div{
            margin: 0 auto;
            width: 400px;
            height: 400px;
            background-color: blanchedalmond;
  /* 背景图片 */
            background-image: url(./图片.jpg);
            /* 默认水平垂直都平铺 
            装饰品不能撑开容器*/
  /* 背景平铺 
            repeat默认的*/
            /* background-repeat:repeat ; */
            /* 不平铺 */
            background-repeat: no-repeat;
            /* x轴平铺 */
            /* background-repeat: repeat-x; */
            /* y轴平铺 */
            /* background-repeat: repeat-y; */
            /* 当容器宽高与背景图片宽高相等时可以省略 */
  /* 背景位置 */
            /* 正居中一个center就行 */
            /* background-position:center;
            background-position: left bottom; */
            /* 数字+px */
            background-position: 50px 50px;
        }
    </style>
</head>
<body>
    <div>我是一个三百</div>
</body>
```

![3](C:\Users\86159\Pictures\3.jpg)

## 9.背景连写    background: 空格 ;

```html
<style>
        div{
            width: 400px;
            height: 400px;
            background: #fff666 url(./图片.jpg) no-repeat 100px bottom;
        }
    </style>
```

## 10.块级元素 block

•    显示特点：

1.   独占一行(一行只能显示一个)

2.   宽度默认是父元素的宽度，高度默认由内容撑开

3.   可以设置宽高

•    代表标签：div、p、  h系列、  ul、  li、dl、dt、dd、form、  header、  nav、footer……

## 11.行内标签 inline

•    显示特点：

1.    一行可以显示多个

2.    宽度和高度默认由内容撑开

3.    不可以设置宽高(不是不让你写，是写了也不生效)

代表标签：a、span 、 b、  u、  i、s、strong、 ins、em、del……

## 12.行内块元素 inline-block

➢  显示特点：

1.    一行可以显示多个

2.    可以设置宽高

 •    代表标签：input、textarea、button、select……

## 13.显示模式转换 display:;

```html
<style>
        body{
          /* 取消文字间距 */
            font-size: 0;
        }
        div{
            /* 转行内快 */
            width: 200px;
            height: 200px;
            background-color: #dd8686;
            display: inline-block;
            font-size: 16px;
        }
        span{
            /* 转块级 */
            width: 100px;
            height: 100px;
            font-size: 16px;
            background-color: #21ae49;
            display: block;
        }
        p{
            /* 转行内 */
            width: 100px;
            height: 100px;
            font-size: 16px;
            background-color: #5028ad;
            display:inline;
        }
    </style>
```

# day05-2.20

## 01.css特性

➢ 继承性：子元素有默认继承父元素样式的特点(子承父业)

​	好处：可以在一定程度上减少代码

•   有些标签有自带的特性：比如标题标签，a标签

•   有哪些常见属性可以继承？

1.    color
2.    font-style、font-weight、font-size、font-family
3.    text-indent、text-align
4.    line-height

➢ 层叠性

•  特性：

1.    给同一个标签设置不同的样式 → 此时样式会层叠叠加 → 会共同作用在标签上

2.    给同一个标签设置相同的样式 → 此时样式会层叠覆盖 → 最终写在最后的样式会生效

## 02.优先级

•  特性：不同选择器具有不同的优先级，优先级高的选择器样式会覆盖优先级低选择器

•  优先级公式:！important>行内样式>id选择器>类选择器>标签选择器>通配符选择器>继承

```html
 <style>
        /* 继承无法添加！important */
        body{
            color: rgb(40, 123, 76);
        }
        .box{
            color: beige;
        }
        #id{
            color: blue;
        }
        *{
            color: red !important;
        }
    </style>
</head>
<body>
    <div class="box" id="two" style="color: aqua;">测试优先级</div>
</body>
```

## 03.权重叠加计算

➢ 场景：如果是复合选择器，此时需要通过权重叠加计算方法，判断最终哪个选择器优先级最高会生效

➢ 权重叠加计算公式：（每一级之间不存在进位）

•  权值相同，谁在后面运行谁

•  都是继承，谁靠内容近运行谁

```html
 <style>
        /* (行内，id，类，标签) */
        /* !important最高 */
        /* （0，2，0，0） */
        #father #son{
            color: blue;
        }
        /* （0，1，1，1） */
        #father p.c2{
            color: aqua;
        }
        /* （0，0，2，2） */
        div.c1 p.c2{
            color: brown;
        }
        /* 继承最低 加!important也没用*/
        #father{
            color: deeppink !important;
        }
    </style>
</head>
<body>
        <div id="father" class="c1">
        <p id="son" class="c2">一段测试文字</p>
    </div>
</body>
```

## 04.盒子模型

➢ 盒子的概念

•  .页面中的每一个标签，都可看做是一个“盒子”，通过盒子的视角更方便的进行布局

•  .浏览器在渲染（显示）网页时，会将网页中的元素看做是一个个的矩形区域，我们也形象的称之为盒子

➢ 盒子模型

•  CSS中规定每个盒子分别由：内容区域（content）、内边距区域（padding）、边框区域（border）、外边距区域（margin）构成，这就是 盒子模型

➢ 盒子的宽高

•  作用：利用 width 和 height 属性默认设置是盒子 内容区域 的大小

•  属性：width/height

•  常见取值：数字+px

➢ 盒子的边框

•  作用：给设置边框粗细、边框样式、边框颜色效果

```html
 <style>
        /* 盒子的内容区域：蓝色 */
        div{
            margin: 0 auto;
            width: 300px;
            height: 300px;
            background-color: #ac4a4a;
            border-width: 10px;
            border-style: solid;
            /* 当没有设置边框颜色的的时候，默认黑色 */
            border-style: dashed;
            border-style: dotted;
            border-color: gold;
            border: 10px dashed gold;
        }
    </style>
```

•  边框粗细	border-width	数字+px

•  边框样式	border-style	solid	实线		dashed虚线		dotted点线

•  边框颜色	border-color

➢ 边框（border）- 单方向设置  border-方向名称

•  场景：只给盒子的某个方向单独设置边框

```html
 border-top: 10px blue solid;
 border-bottom: 10px yellow dashed;
 border-left:10px pink dotted;
 border-right: 10px #fff dashed
```

➢ 盒子实际大小初级计算公式：

•   盒子宽度=左边框+内容宽度+右边框

•   盒子高度=上边框+内容高度+下边框

•   解决：当盒子被border撑大后,计算多余大小，手动在宽高中减去。

➢ 盒子尺寸 400*400，背景绿色，边框10px 实线 黑色

```html
<style>
        div{
            width: 380px;
            height: 380px;
            border: 10px solid;
        }
    </style>
```

## 05.内边距 padding

•   作用：设置边框 与 内容区域 之间的距离

➢ 内边距（padding）- 单方向设置	

•   属性名：padding-方位名词	属性值：数字+px

```html
<style>
        div{
            width: 300px;
            height: 300px;
            background-color: #a04e4e;
            /* 四周 */
            padding: 10px;
            /* 上下，左右 */
            padding: 5px 10px;
            /* 上，左右，下 */
            padding:5px 10px 15px ;
            /* 上，右，下，左 */
            padding:5px 10px 15px 20px ;
            padding: 5px 0 0 5px;
            /* top bottom left right */
            padding-top: 20px;
            padding-bottom:20px ;
        }
    </style>
```

盒子实际大小终极计算公式

➢ 需求：盒子尺寸300*300，背景粉色，边框10px实线黑色，上下左右20px的内边距，如何完成？

•   注意点：①设置width和height是内容的宽高！②设置border会撑大盒子③设置padding会撑大盒子

➢ 盒子实际大小终极计算公式：

•   盒子宽度= 左边框+ 左padding +内容宽度+右padding +右边框

•   盒子高度= 上边框+ 上padding +内容宽度+下padding +下边框

➢  解决：当盒子被border和padding撑大后，如何满足需求？

•    自己计算多余大小，手动在内容中减去（手动内减）

```html
 <style>
        div{
            width: 240px;
            height: 240px;
            border: 10px solid;
            padding: 20px;
            background-color: pink;
        }
    </style>
```

➢ 不会撑大盒子的特殊情况（块级元素）

1.如果子盒子没有设置宽度，此时宽度默认是父盒子的宽度

2.此时给子盒子设置左右的padding或者左右的border，此时不会撑大子盒子

## 06.自动内减  box-sizing:border-box;

➢  解决方法 ① ：手动内减

•   操作：自己计算多余大小，手动在内容中减去

•   缺点：项目中计算量太大，很麻烦

➢  解决方法②：自动内减

•   操作：给盒子设置属性box-sizing: border-box;即可

•   优点：浏览器会自动计算多余大小，自动在内容中减去

```html
 <style>
        div{
            width: 300px;
            height: 300px;
            border: 10px solid;
            padding: 20px;
            background-color: #21c5a7;
            /* box-sizing: border-box; */
           /* 不加360*360 加上300*300 */
        }
    </style>
```

## 07.内边距 padding

•   作用：设置边框 与 内容区域 之间的距离

•   记忆规则：从上开始赋值，然后顺时针赋值，如果设置赋值的，看对面的！！

```html
<style>
        div{
            width: 300px;
            height: 300px;
            background-color: #a04e4e;
            /* 四周 */
            padding: 10px;
            /* 上下，左右 */
            padding: 5px 10px;
            /* 上，左右，下 */
            padding:5px 10px 15px ;
            /* 上，右，下，左 */
            padding:5px 10px 15px 20px ;
            padding: 5px 0 0 5px;
            /* top bottom left right */
            padding-top: 20px;
            padding-bottom:20px ;
        }
    </style>
```

➢   内边距（padding）- 单方向设置

•   场景：只给盒子的某个方向单独设置内边距

•   属性名：padding-方位名词

•   属性值：数字+px

## 08.盒子实际大小终极计算公式

•   需求：盒子尺寸300*300，背景粉色，边框10px实线黑色，上下左右20px的内边距，如何完成？

•   注意点：①设置width和height是内容的宽高！②设置border会撑大盒子③设置padding会撑大盒子

➢   盒子实际大小终极计算公式：

•   盒子宽度= 左边框+ 左padding +内容宽度+右padding +右边框

•   盒子高度= 上边框+ 上padding +内容宽度+下padding +下边框

•   解决：当盒子被border和padding撑大后，如何满足需求？

自己计算多余大小，手动加减

```html
<style>
        div{
            width: 240px;
            height: 240px;
            border: 10px solid;
            padding: 20px;
            background-color: pink;
        }
    </style>
```

➢   不会撑大盒子的特殊情况（块级元素）

1.如果子盒子没有设置宽度，此时宽度默认是父盒子的宽度

2.此时给子盒子设置左右的padding或者左右的border，此时不会撑大子盒子

➢   CSS3盒模型（自动内减）

•   操作：给盒子设置属性box-sizing: border-box;即可

•   优点：浏览器会自动计算多余大小，自动在内容中减去

```html
<style>
        div{
            width: 300px;
            height: 300px;
            border: 10px solid;
            padding: 20px;
            background-color: #21c5a7;
            /* box-sizing: border-box; */
            /* 不加360*360 加上300*300 */
        }
    </style>
```

## 09.外边距 margin

•   作用：设置边框以外，盒子与盒子之间的距离

➢   清除默认内外边距外边距（margin） - 单方向设置

•   场景：只给盒子的某个方向单独设置外边距

•   属性名：margin - 方位名词

•   属性值：数字 + px

```html
div{
            width: 200px;
            height: 200px;
            background-color: #952929;
            margin: 10px;
            /* 上下，左右 */
            margin: 10px 15px ;
            /* 上，左右，下 */
            margin: 10px 15px 20px;
            /* 上，右 ，下，左25 */
            margin: 10px 15px 20px 20px;
            /* top bottom left right */
            margin-top:10px ;
        }
```

➢   清除默认内外边距

•   场景：浏览器会默认给部分标签设置默认的margin和padding，但一般在项目开始前需要先清除这些标签默认的margin和padding，后续自己设置

•   比如：body标签默认有margin：8px

•   比如：p标签默认有上下的margin

•   比如：ul标签默认由上下的margin和padding-left

## 10.盒子特殊情况

➢   外边距正常情况

•   场景：水平布局 的盒子，左右的margin正常，互不影响

•   结果：最终两者距离为左右margin的和

➢   外边距折叠现象 – ① 合并现象

•   场景：垂直布局的 块级元素，上下的margin会合并

•   结果：最终两者距离为margin的最大值

•   解决方法：避免就好只给其中一个盒子设置margin即可

➢   外边距折叠现象 – ② 塌陷现象

•   场景：互相嵌套 的**块级**元素，子元素的 margin-top会作用在父元素上

•   结果：导致父元素一起往下移动

•   解决方法：

1.给父元素设置border-top或者 padding-top（分隔父子元素的margin-top）

2.给父元素设置overflow：hidden ;溢出隐藏

3.转换成行内块元素

4.设置浮动

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        div{
            width: 300px;
            height: 300px;
            background-color: pink;
            /* margin-top: 10px; */
            /* padding-top: 20px;
            box-sizing: border-box; */
            /* 1 */
            /* transparent透明 */
            /* border-top: 1px solid transparent;
            box-sizing: border-box; */
            /* 2 */
            /* padding-top: 1px; */
            /* 3 */
            /* overflow: hidden; */
        }
        p{
            width: 100px;
            height: 100px;
            background-color: green;
            margin-top: 20px;
            /* 4 */
            /* display: inline-block; */
            /* 5 */
            /* float: left; */
        }
    </style>
```

➢  行内元素的margin和padding

•   场景：给行内元素设置margin和padding时

•   结果：

1.水平方向的margin和padding布局中有效！

2.垂直方向的margin布局中无效！

# day06-2.21

## 01-结构伪类选择器

➢  作用与优势：

1.作用：根据元素在HTML中的结构关系查找元素

2.优势：减少对于HTML中类的依赖，有利于保持代码整洁

3.场景：常用于查找某父级选择器中的子元素

•   注意父级元素后面要加空格或者子代选择器>

E :first-child{}	E :last-child{}	E :nth-child(n){}	E :nth-last-child(n){}

```html
 <style>
        /* 第一个子集 */
        ul :first-child{
            color: aqua;
        }
        /* 最后一个子集 */
        ul :last-child{
            color: blue;
        }
        /* 任意子集 */
        ul>:nth-child(3){
            background-color: gold;
        }
        /* 倒数第几个子集 */
        ul>:nth-last-child(2){
            background-color: green;
        }
    </style>
```

➢ n的注意点：

1. n为：0、1、2、3、4、5、6、……

2. 通过n可以组成常见公式:偶数2n,奇数2n-1,5n

```html
<style>
        /* 
        -n+?    找前几个子集
        n+？     找到从第几个往后
        */
        ul>:nth-child(2n){
            background-color: gold;
        }
    </style>
```

## 02.nth-of-type结构伪类选择器

E ：nth-of-type(n){} 	只在父元素的同类型子元素范围内

```html
<style>
        div>:nth-child(1){
            color: red;
        }
        div>span:nth-of-type(1){
            color: brown;
        }
    </style>
```

## 03.伪元素

➢  伪元素：一般页面中的非主体内容可以使用伪元素

➢  区别：

1.元素：HTML设置的标签

2.伪元素：由CSS模拟出的标签效果

➢  注意点：

1.必须设置content属性才能生效

2.伪元素默认是行内元素

3.伪元素创建出来后默认的显示模式是行内元素

```html
<style>
        p::before{
            content:"老鼠";
            color: gold;
            display: inline-block;不加这句宽高不能显示
            width: 100px;
            height: 100px;
            background-color: green;
        }
        p::after{
            content:"大米";
        }
        /* 选中文本首字母 */
        div::first-letter{
            font-size: 30px;
        }
        /* 文本第一行 */
        div::first-line{
            color: pink;
        }
        /* 改变文本选中的状态 可以直接作用于全文（删去div）*/
        div::selection{
            background-color: aqua;
            color: blue;
        }
    </style>
```

```html
    <style>
        p::after{
            content: "\e606";字体图标的代码
            font-family: 'iconfont' !important;	字体显示
            font-size: 20px;
            color: #000;
        }

    <style>
</head>
<body>
    <p>我的</p>
</body>

```



## 04.标准流

➢ 标准流：又称文档流，是浏览器在渲染显示网页内容时默认采用的一套排版规则，规定了应该以何种方式排列元素

➢ 常见标准流排版规则：

1.块级元素：从上往下，垂直布局，独占一行

2.行内元素或行内块元素：从左往右，水平布局，空间不够自动折行

## 05.浮动	float

•   作用：早期的作用：图文环绕；网页布局

•   代码：1.左浮动：float:left

​	    2.右浮动：float:right

•   特点：

1.浮动元素会脱离标准流（简称：脱标），在标准流中不占位置

2.浮动元素比标准流高半个级别，可以覆盖标准流中的元素

3.浮动找浮动，下一个浮动元素会在上一个浮动元素后面左右浮动

4.浮动元素有特殊的显示效果：一行可以显示多个，可以设置宽高

•   注意点：浮动的元素不能通过text-align:center或者margin:0auto

# day07-2.22

## 书写网页导航步骤

1.清除默认的margin和padding

2.找到ul，去除小圆点

3.找到li标签，设置浮动让li一行中显示

4.找到a标签，设置宽高→a标签默认是行内元素，默认不能设置宽高？？

•   方法一：给a标签设置display: inline-block

•   方法二：给a标签设置display:block

•   方法三：给a设置float:left

## 01.清除浮动带来的影响

➢ 含义：清除浮动带来的影响

•   影响：如果子元素浮动了，此时子元素不能撑开标准流的块级父元素

➢ 原因：

•   子元素浮动后脱标→不占位置

➢ 目的：需要父元素有高度，从而不影响其他网页元素的布局

➢ 直接设置父元素高度

•   优点：简单粗暴，方便

•   缺点：有些布局中不能固定父元素高度。如：新闻列表、京东推荐模块

➢ 额外标签法

1.在父元素内容的最后添加一个块级元素

2.给添加的块级元素设置clear:both

•   缺点：会在页 面中添加额外的标签，会让页面的HTML结构变得复杂

```html
p{
            clear:both;
        }
```

➢ 单伪元素清除法

•   操作：用伪元素替代了额外标签			.clearfix是父辈元素的类名

•   优点：项目中使用，直接给标签加类即可清除浮动

```
.clearfix::after{
            content:"";
            display: block;
            clear: both;
            height: 0;
            visibility: hidden;
        }
```

➢  双伪元素清除法

•  优点：项目中使用，直接给标签加类即可清除浮动

➢  给父元素设置overflow : hidden

•  直接给父元素设置overflow: hidden；

```html
<style>
        .box{
            width: 200px;
            height: 200px;
            background-color: green;
        }
        p{
            clear:both;
        }
        .son{
            float: left;
            width: 100px;
            height: 300px;
            background-color: red;
        }
        /* 单伪元素清除法 */
        .clearfix::after{
            content:"";
            display: block;
            clear: both;
            height: 0;
            visibility: hidden;
        }
        /* 双伪元素清除法 */
        .clearfix::after,.clearfix::before{
            content: "";
            display: table;
        }
        .clearfix::after{
            clear: both;
        }
        /* 
            BFC块级格式化上下文
            实现方法：
                1.浮动
                2.定位
                3.overflow:hidden auto visible无法实现
                4.根元素html就是一个bfc    
                5.display；inline-blockinline-block
        */
    </style>
</head>
<body>
    <div class="box clearfix">
        <div class="son"></div>
        <!-- 方法二 额外标签法 -->
        <p></p>
    </div>
```

## 02.定位	position:;

➢  静态定位	static

•   介绍：静态定位是默认值，就是之前认识的标准流

➢  相对定位	relative

•   自恋型定位，相对于自己之前的位置进行移动

•   特点：

1. 需要配合方位属性实现移动


2. 相对于自己原来位置进行移动


3. 在页面中占位置→没有脱标

```html
<style>
        div{
            width: 200px;
            height: 200px;
            background-color: pink;
            /* 相对定位 */
            position: relative;
            left: 30px;
            top: 80px;
        }
    </style>
```

➢  绝对定位	absolute

•   拼爹型定位，相对于非静态定位的父元素进行定位移动

•   特点：

1. 需要配合方位属性实现移动
2. 默认相对于浏览器可视区域进行移动
3. 在页面中不占位置 → 已经脱标

```html
<style>
        div{
            width: 200px;
            height: 200px;
            background-color: pink;
            /* 相对定位 */
            position:absolute;
            left: 30px;
            top: 10px;
        }
    </style>
```

➢  固定定位	fixed

•   介绍：死心眼型定位，相对于浏览器可视画面进行定位移动

•   特点：

1. 需要配合方位属性实现移动
2. 相对于浏览器可视区域进行移动
3. 在页面中不占位置→已经脱标

•   应用场景：让盒子固定在屏幕中的某个位置

➢  粘性定位 	sticky

一定需配合方向词使用，类似固定定位，占位，吸顶效果

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        header{
            height: 20px;
            background-color: gold;
            /* position: fixed; */
            /* width: 100%; */
            /* 粘性定位
            不脱标
            占位 */
            position: sticky;
            top: 0;
        }
        section{
            height: 2000px;
            background-color: pink;
        }
        div{
            width: 80px;
            height: 80px;
            background-color: red;
            /* 固定定位 */
            position: fixed;
            top: 100px;
        }
    </style>
```

## 03.父相子绝

➢  场景：让子元素相对于父元素进行自由移动

➢  含义：

•  子元素：绝对定位

•   父元素：相对定位

➢  子绝父相好处：

•   父元素是相对定位，则对网页布局影响最小

➢  子绝父绝特殊场景

•   场景：在使用子绝父相的时候，发现父元素已经有绝对定位了，此时直接子绝即可！

•   原因：父元素已经有定位已经满足要求，如果盲目修改父元素定位方式，可能会影响之前写好的布局

## 04元素层级	z-index:;

场景：改变定位元素的层级

属性值：数字

•  数字越大，层级越高

## 05.垂直对齐方式	vertical-align:;

➢  场景：解决行内/行内块元素垂直对齐问题

➢  问题：当图片和文字在一行中显示时，其实底部不是对齐的

| 属性值      | 效果      |
| -------- | ------- |
| baseline | 默认，基线对齐 |
| top      | 顶部对齐    |
| middle   | 中部对齐    |
| bottom   | 底部对齐    |



➢  vertical-align 可以解决的问题

•   文本框和表单按钮无法对齐问题

•   input和img无法对齐问题

•   div中的文本框，文本框无法贴顶问题

•   div不设高度由img标签撑开，此时img标签下面会存在额外间隙问题

•   使用line-height让img标签垂直居中问题

➢  outline 取消浏览器页面中选中时出现的样式

outline:none;

## 06.光标类型	cursor

➢  场景：设置鼠标光标在元素上时显示的样式(default)

```html
<style>
        div{
            width: 200px;
            height: 200px;
            background-color: aqua;
            /* 小手效果 */
            cursor:pointer ;
            /* 工字型 */
            cursor:text;
            /* 十字光标 */
            cursor: move;
        }
    </style>
```

## 07.边框圆角 	border-radius

•   场景：让盒子四个角变得圆润，增加页面细节，提升用户体验

•   属性名：border-radius

•   常见取值：数字+px 、百分比

•   赋值规则：从左上角开始赋值，然后顺时针赋值，没有赋值的看对角

```html
 <style>
        .bb{
            width: 100px;
            height: 100px;
            background-color: aqua;
            margin: 200px auto;
            /* 四个角 */
            border-radius:10px ;
            /* 左下 */
            border-bottom-left-radius: 20px;
            /* 左上，右下      右上，左下 */
            border-radius: 10px 20px;
            /* 左上，右上 左下，右下 */
            border-radius: 20px 30px 40px;
            /* 左上，右上，右下 ，左下*/
            border-radius: 10px 15px 20px 30px;
            /* 百分比 */
            /* 正方形变圆 */
            border-radius: 50%;
        }
        .sb{
            width: 300px;
            height: 100px;
            background-color: red;
            margin: auto;
            /* 椭圆 */
            border-radius: 50%;
            /* 胶囊型 */
            border-radius: 50px;
        }
        button{
            width: 100px;
            height: 50px;
            border: 0;
            background-color: gold;
            border-radius: 50%;
        }
    </style>
```



## 08.溢出	overflow

•   溢出部分：指的是盒子 内容部分 所超出盒子范围的区域

•   场景：控制内容溢出部分的显示效果，如：显示、隐藏、滚动条……

```html
<style>
        div{
            width: 100px;
            height: 100px;
            background-color: aqua;
           /* 默认值，溢出部分可见 */
          overflow:visible;
            /* 溢出隐藏; */
            overflow: hidden;
            /* 无论是否溢出，都产生滚动条 */
            overflow: scroll;
           /* 根据是否溢出，自动显示或者隐藏滚动条 */
           overflow: auto;
        }
        /* 取消滚动条 */
        div::-webkit-scrollbar{
            display: none;
        }
    </style>
```

## 09.隐藏	visibility

➢  常见属性：

1.visibility：hidden

2.display：none

➢  区别：

1.visibility：hidden 隐藏元素本身，并且在网页中占位置

2.display：none 隐藏元素本身，并且在网页中不占位置

➢  注意点：

•    开发中经常会通过display属性完成元素的显示隐藏切换

display：none；（隐藏）、display：block；（显示）

## 10.透明度	opacity

•   场景：让某元素整体（包括内容）一起变透明

➢  属性值：

•   0~1之间的数字

•   1：表示完全不透明

•   0：表示完全透明

## 11.遮罩

给全局做一个遮罩，需加一个div标签（body的子代），添加固定定位，宽高100%，遮罩如果有内容不要用opacity

```less
.zhe{
    position: fixed;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    top: 0;
    z-index: 1;
    div{
        width: (320 / @vw);
        height: (100 / @vw);
        position: absolute;
        top: (260 / @vw);
        left: (31 / @vw);
        color: #3C3C3C;
        font-size: (16 / @vw);
        background-color: white;
        opacity: 1;
        p{
            width: (320 / @vw);
            height: (50 / @vw);
            text-align: center;
            line-height: (50 / @vw);
        }
        p:nth-of-type(1){
            border-bottom: 1px solid #C8C8C8;
        }
    }
}  

<body>
  
        <div class="zhe">
            <div>
                <p>拍摄照片</p>
                <p>从手机相册选择</p>
            </div>
        </div>
</body>
```



# day09-2.24

## 01.链接伪类选择器

•   场景：常用于选中超链接的不同状态同时实现以上四种伪类状态效果，按照 LVHA 顺序书写

```html
<style>
        /* 未访问过的状态 */
        a:link{
            background-color: aqua;
        }
        /* 访问之后的状态 */
        a:visited{
            background-color: pink;
        }
        /* 鼠标悬停 */
        a:hover{
            background-color: green;
        }
        /* 鼠标按下 */
        a:active{
            background-color: blue;
        }
    </style>
```

## 02.焦点伪类选择器	:focus

•   场景：用于选中元素获取焦点时状态，常用于表单控件

•   表单控件获取焦点时默认会显示外部轮廓线		后面可以加上outline:none;

```html
<style>
        input{
            width: 100px;
            height: 20px;
            /* border: 0; */
            outline: none;
        }
        input:focus{
            background-color: aqua;
        }
    </style>
```

## 03.属性选择器【】

•   场景：通过元素上的HTML属性来选择元素，常用于选择 input 标签

```html
<style>
        input[type]{
            background-color: pink;
        }
        input[type="password"]{
            background-color: gold;
        }
        div[class]{
            background-color: green;
        }
    </style>
```

## 04.精灵图/图片整合

•   场景：项目中将多张小图片，合并成一张大图片，这张大图片称之为精灵图

•   优点：减少服务器发送次数，减轻服务器的压力，提高页面加载速度

➢  精灵图的使用步骤

•   创建一个盒子

•   通过ps量取小图片大小，将小图片的宽高设置给盒子

•   将精灵图设置为盒子的背景图片

•   通过ps测量小图片左上角坐标，分别取负值设置给盒子的background-position：x y；

```html
<style>
        section{
            margin: 200px auto;
        }
        article{
            width: 24px;
            height: 24px;
            background:url(./img/精灵图2.jpg) ;
        }
        div{
            width: 24px;
            height: 24px;
            background:url(./img/精灵图2.jpg) 0 -88px;
            /* background-position: 0 0; */
        }
    </style>
```



## 05.背景图片大小	background-size

•   作用：设置背景图片的大小，

•   语法：background-size：宽度 高度；

```html
<style>
        div{
        width: 300px;
        height: 200px;
        background-color: aqua;
        background-image: url(./img/3.jpg);
        background-repeat: no-repeat;
        /* 图片宽高100px */
        background-size: 100px;
        /* 当前盒子自身的宽高百分比 */
        background-size:70% ;
        /* 包含，将图片等比例缩放，直到盒子能包含的最大*/
        background-size: contain;
        /* 填满整个盒子 ，不是等比缩放*/
        background-size: cover;
        /* 连写 */
        background: red url(./img/3.jpg) no-repeat center/200px 200px;
        }
    </style>
```

➢  连写

•   注意点：background-size和background连写同时设置时，需要注意覆盖问题解决：

1.要么单独的样式写连写的下面

2.要么单独的样式写在连写的里面

## 06.文字阴影	text-shadow

•   作用：给文字添加阴影效果，吸引用户注意

•   阴影可以叠加设置，每组阴影取值之间以逗号隔开

```html
<style>
        div{
            /* 水平位置，垂直位置，模糊度，颜色 */
            text-shadow: 8px 8px 0.3px gold,15px 15px 0.5px red;
        }
    </style>
```

## 07.盒子阴影	box-shadow

•   作用：给盒子添加阴影效果，吸引用户注意，体现页面的制作细节

| 参数       | 作用            |
| -------- | ------------- |
| h-shadow | 必须，水平偏移量。允许负值 |
| v-shadow | 必须，垂直偏移量。允许负值 |
| blur     | 可选，模糊度        |
| spread   | 可选，阴影扩大       |
| color    | 可选，阴影颜色       |
| inset    | 可选，将阴影改为内部阴影  |



```html
<style>
        div{
            width: 300px;
            height: 300px;
            margin: auto;
            box-shadow: 10px 10px 3px 10px gold inset，10px 10px 3px 10px gold;
        }
    </style>
```

## 08.过渡	transition

•   作用：让元素的样式慢慢的变化，常配合hover使用，增强网页交互体验

•   注意点：

1.过渡需要：默认状态 和 hover状态样式不同，才能有过渡效果

2.transition属性给需要过渡的元素本身加

3.transition属性设置在不同状态中，效果不同的

①  给默认状态设置，鼠标移入移出都有过渡效果

②  给hover状态设置，鼠标移入有过渡效果，移出没有过渡效果

```html
<style>
        div{
            width: 200px;
            height: 200px;
            background-color: gold;
            transition:all 2s linear;
        }
        div:hover{
            width: 40px;
            height: 30px;
            background-color: aqua;
        }
    </style>
```

## 

# day10-2.27



## 01-字体图标

➢  目标：使用字体图标技巧实现网页中简洁的图标效果!

设置大小用font-size

➢  字体图标的优点：

•   权重比较高

•   灵活性：灵活地修改样式，例如：尺寸、颜色等

•   轻量级：体积小、渲染快、降低服务器请求次数

•   兼容性：几乎兼容所有主流浏览器

•   使用方便：

1.下载字体包

2.使用字体图标

•   图标库	lIconfont：https://[www.iconfont.cn/](http://www.iconfont.cn/)

```html
<link rel="stylesheet" href="./day-10/font_gb9pc9b629u/iconfont.css">
    <style>
        /* 注意权重 */
        .icon-gongneng{
            color: gold;
            font-size: 30px;
        }
        /* 需要加字体样式iconfont */
        div{
            font-family: iconfont;
        }
    </style>
</head>
<body>
    <span class="iconfont icon-gongneng"></span>
    <span class="iconfont icon-wode"></span>
    <div>&#xe7d0;</div>
</body>
```

## 02-购物车案例

•   布局标签	li> span*3

•   字体图标	

1.引入字体图标样式表

2.购物车和箭头span调用字体图标类名



## 03-容器正居中

•   目标：使用translate快速实现绝对定位的元素居中效果

添加旋转效果时别用

```html
<style>
        .box{
            width: 300px;
            height: 300px;
            background-color: red;
            position: relative;
        }
        .box div{
            width: 100px;
            height: 100px;
            background-color: gold;
            position: absolute;
            /* 父级的一半 */
            left: 50%;
            top: 50%;
            /* 自身的一半 */
           transform: translate(-50%,-50%);
        }
    </style>
```



## 04-位移案例

•   使用translate实现元素位移效果

```html
<style>
        .box{
            width: 400px;
            height: 200px;
            margin: 200px auto;
            border: 1px solid;
            /* 溢出隐藏 */
            overflow: hidden;
        }
        .left{
            width: 200px;
            height: 200px;
            background-color: gold;
            float: left;
        }
        .right{
            width: 200px;
            height: 200px;
            background-color: goldenrod;
            float: right;
        }
        .box:hover .left{
            transform: translate(-100%);
            transition: all 1.5s linear;
        }
        .box:hover .right{
            transform: translate(100%);
            transition: all 1.5s linear;
        }
    </style>
</head>
<body>
    <div class="box">
        <div class="left"></div>
        <div class="right"></div>
    </div>
</body>
```

## 05-双开门案例

```html
 <style>
        *{
            margin: 0;
            padding: 0;
        }
        .box{
            margin: 100px auto;
            overflow: hidden;
            width: 1366px;
            height: 600px;
            background: url(./img/original_f9d9c123c62c1df29ca54e5b3b8e82d3.jpg);
            overflow: hidden;
        }
        .box :first-child,
        .box :last-child{
            float: left;
            transition: all 1.5s linear;
            width: 50%;
            height: 600px;
            background: url(./img/original_551a2f971e463d59871dc8e7bd4af025.jpg);
        }
        .box :last-child{
            background: url(./img/original_551a2f971e463d59871dc8e7bd4af025.jpg) right;
        }
        .box:hover :first-child{
            transform: translate(-100%);
        }
        .box:hover :last-child{
            transform: translate(100%);
        }
    </style>
</head>
<body>
    <div class="box">
        <div></div>
        <div></div>
    </div>
</body>
```

## 06-双开门案例2	用伪元素

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        div{
            width: 1366px;
            height: 600px;
            margin: 200px auto;
            background-image: url(./img/original_f9d9c123c62c1df29ca54e5b3b8e82d3.jpg);
        }
        div::before,
        div::after{
            content: "";
            display: block;
            width: 50%;
            height: 100%;
            background: url(./img/original_551a2f971e463d59871dc8e7bd4af025.jpg);
            transition: all 1.5s linear;
            float: left;
        }
        div::after{

            background-position: right 0;
        }
        div:hover::after{
            transform: translate(100%);
        }
        div:hover::before{
            transform: translate(-100%);
        }
    </style>
</head>
<body>
    <div></div>
</body>
```



## 07-旋转transform:rotate();

➢  使用rotate实现元素旋转效果（写在伪类选择器hover内）

•   语法transform:rotate(角度);  注意：角度单位是deg

•   技巧：取值正负均可

1.取值为正,则顺时针旋转

2.取值为负,则逆时针旋转

➢  使用transform-origin属性改变转换原点（写在标签选择器）

•   默认圆点是盒子中心点

•   transform-origin: 原点水平位置 原点垂直位置

取值：

1.方位名词（left、top、right、bottom、center）

2.像素单位数值

3.百分比（参照盒子自身尺寸计算）

```html
 <style>
        img{
            width: 200px;
            display: block;
            margin: 100px auto;
            background:pink;
            transition: all 2s linear;
            /* transform-origin: left top; */
            /* transform-origin: right bottom; */

            /* 只设置一个方向词，围绕当前边的中心点旋转 */
            /* transform-origin: left; */
            /* transform-origin: top; */

            /* transform-origin: 100px 100px; */
            /* transform-origin: -100px -100px; */

            /* transform-origin: 50% 50%; */
            /* transform-origin: -50% -50%; */
        }
        img:hover{
            /* transform-origin: right bottom; */
            transform: rotate(-360deg);

        }
```

注意：给图片添加旋转效果时，不能给图片垂直居中用父相子绝+tranform:translate(-50%,-50%)

```less
text-align: center;
                img{
                    vertical-align: middle;                 
                    transition: all 1.5s linear;                                      
                }
```



## 08-位移旋转

```html
<style>
        div{
            width: 900px;
            height: 300px;
            border: 3px solid;           
        }
        img{
            transition: all 3s linear;
        }
        div:hover img{     
                /* 位移要写前面 */
            transform: translate(600px) rotate(360deg) ;
        }
    </style>
</head>
<body>
    <div>
        <img src="./img/轮胎.png" alt="">
    </div>
</body>
```

## 09-缩放	transform:scale(数字)；

•   目标：使用scale改变元素的尺寸

•   scale值大于1表示放大, scale值小于1表示缩小

```html
<style>
        div{
            width: 200px;
            height: 200px;
            margin: 200px auto;
            background-color: pink;
            overflow: hidden;
        }
        img{
            width: 100%;
            height: 100%;
            transition: all 2s linear;
        }
        div:hover img{
            transform: scale(1.5);
        }
    </style>
```



## 10-和平精英案例

```html
<style>
        .box{
            width: 300px;
            height: 250px;
            margin: 200px auto;
            background-color: aqua;
        }
        .box>div :first-child{
            width: 300px;
            height: 150px;
        }
        .box div{
            width: 100%;
            height: 150px;
            position: relative;
        }
        /* 注意transform的层叠型 */
        .box>div :last-child{
            position: absolute;
            left: 50%;
            top: 50%;
            transform: translate(-50%,-50%) scale(5);
            transition: all 1.5s linear;
            opacity: 0;
        }
        .box>div:hover :last-child{
            opacity: 1;
            transform: translate(-50%,-50%) scale(1);
        }
        p{
            padding: 0 10px;
        }
    </style>
</head>
<body>
    <div class="box">
        <div>
            <img src="./img/和平精英.jpeg" alt="">
            <img src="./img/anniu.png" alt="">
        
        </div>
        <p>
            公司成立于1984年，
            经过近30年的发展
            已成为电气制造，房地产开发和金融
            投资三业并举的综合性跨国…</p>
    </div>
```

## 11-渐变	linear-gradient

•   目标：使用background-image属性实现渐变背景效果

•   显示两种或多种指定颜色之间的平滑过渡

```html
<style>
        div{
            width: 300px;
            height: 200px;
            margin: 200px auto;
            /* 注意两颜色之间用，隔开  默认从上到下 */
            background-image: linear-gradient(gold,red);
            /* 从左到右 四个方向词 */
            background-image: linear-gradient(to right,gold,red,blue);
            /* 从左上到右下 对角 */
            background-image: linear-gradient(to right bottom,gold,red,blue);
        }
    </style>
```

```html
<style>
        div{
            width: 500px;
            height: 400px;
            margin: 100px auto;
            border-radius: 50%;
            /* 径向渐变circle圆 */
            background-image: radial-gradient(circle,gold,aqua,pink);
            /* 占比 */
            background-image: radial-gradient(circle,black 10%,aqua 10%,pink 60%);
            /* 重复径向渐变 */
            background-image: repeating-radial-gradient(red,aqua 10%,pink 10%);
        }
    </style>
```

# day11-2.28

## 空间转换

•   目标：使用transform属性实现元素在空间内的位移、旋转、缩放等效果

•   空间：是从坐标轴角度定义的。 x 、y 和z三条坐标轴构成了一个立体空间，z轴位置与视线方向相同。

•   空间转换也叫3D转换

•   属性：transform

## 01-空间转换-位移	

•   目标：使用translate实现元素空间位移效果

•   语法

ltransform:translateX(值);

ltransform:translateY(值);

ltransform:translateZ(值);

ltransform:translate3d(x, y,z);

取值（正负均可）像素单位数值	百分比

```html
<style>
        .father{
            perspective: 300px;
        }
        .son{
            width: 200px;
            height: 200px;
            background-color: gold;
            margin: 200px auto;
            transition: all 1.5s linear;
        }
        div:hover{
            transform:translate3d(100px,10px,100px) ;
        }
    </style>
```



## 02-空间转换-透视	perspective：；

•   目标：使用perspective属性实现透视效果

•   属性（添加给父级）

perspective: 数字+px;

取值：像素单位数值，数值一般在800 – 1200。

作用空间转换时，为元素添加近大远小、近实远虚的视觉效果

```html
.father{
            perspective: 300px;
        }
```



## 03-空间转换-旋转	transform:rotateX(数字+deg)

•   目标：使用rotate实现元素空间旋转效果

•   语法

transform:rotateZ(值);

transform:rotateX(值);

transform:rotateY(值);

•   左手法则

判断旋转方向: 左手握住旋转轴, 拇指指向正值方向, 手指弯曲方向为旋转正值方向

•   拓展

1.rotate3d(x,y,z,角度度数)：用来设置自定义旋转轴的位置及旋转的角度

2.x，y，z取值为0-1之间的数字

```html
<style>
        body{
            perspective: 800px;
        }
        div{
            width: 300px;
            height: 300px;
            background-color: gold;
            
        }
        img{
            transition: all 2S linear;
        }
        div:hover img{
            transform: rotateY(360deg);
        }
    </style>
```



## 04-3D导航	transform-style: preserve-3d

目标： 使用transform-style: preserve-3d呈现立体图形

呈现立体图形步骤

1.盒子父元素添加transform-style: preserve-3d；

2.按需求设置子盒子的位置（位移或旋转）

注意:空间内，转换元素都有自已独立的坐标轴，互不干扰

```html
目标：使用立体呈现技巧实现3D导航效果
<style>
        *{
            margin: 0;
            padding: 0;
        }
        a{
            text-decoration: none;
        }
        ul{
            width: 300px;
            height: 50px;
            list-style: none;
            margin: 200px auto;
        }
        li{
            width: 100px;
            height: 50px;
            float: left;
            line-height: 50px;
            text-align: center;
            position: relative;
            /* 呈现立体图形 */
            transform-style: preserve-3d;
            transition: all 1.5s linear;
            /* transform: rotateX(-20deg) rotateY(30deg); */
        }
        a{
            display: block;
            width: 100px;
            height: 50px;
            /* 两个a标签重叠了 */
            position: absolute;
            left: 0;
            top: 0;
        }
        li a:nth-of-type(1){
            background-color: orange;
            /* 注意位移translate单位px  旋转单位deg */
            transform: translateY(-25px) rotateX(90deg);
        }
        li a:nth-of-type(2){
            background-color: green;
            transform: translateZ(25px);
        }
        li:hover{
            transform: rotateX(-90deg);
        }
    </style>
</head>
<body>
    <ul>
        <li>
            <a href="">index</a>
            <a href="">首页</a>
        </li>
        <li>
            <a href="">index</a>
            <a href="">首页</a>
        </li>
        <li>
            <a href="">index</a>
            <a href="">首页</a>
        </li>
    </ul>
</body>
```

## 05-魔方案例

```html
 <style>
        ul{
            width: 200px;
            height: 200px;
            position: relative;
            list-style: none;
            margin: 200px auto;
            transform-style: preserve-3d;
            transition: all 3s linear;
            transform: rotateX(-20deg) rotateY(30deg);	作用：魔方倾斜，方便观看情况
        }
        li{
            width: 200px;
            height: 200px;
            font-size: 50px;
            text-align: center;
            line-height: 200px;
            position: absolute;
            border: 1px solid;
            border-radius: 10px;
            
        }
        ul li:nth-last-of-type(1){
            background-color: gold;
            transform: translateZ(100px);
        }
        ul li:nth-last-of-type(2){
            background-color: pink;
            transform: translateZ(-100px);
        }
        ul li:nth-last-of-type(3){
            background-color: aqua;
            transform: translateY(-100px) rotateX(90deg);
        }
        ul li:nth-last-of-type(4){
            background-color: purple;
            transform: translateY(100px) rotateX(-90deg);
        }
        ul li:nth-last-of-type(5){
            background-color:red ;
            transform: translateX(-100px) rotateY(-90deg);
        }
        ul li:nth-last-of-type(6){
            background-color:green ;
            transform: translateX(100px) rotateY(90deg);
        }
        ul:hover{
            transform: rotate3d(0.2,0.3,0.5,360deg);
        }
    </style>
```

## 06-动画

•   目标：使用animation添加动画效果



```html
<style>
        div{
            width: 200px;
            height: 200px;
            margin: 100px auto;
            animation: dong 2s linear;
        }
  /* 两个状态之间 */
        @keyframes dong {
            from{
                background-color: gold;
            }
            to{
                background-color: aqua;
                width: 300px;
                height: 300px;
            }
        }
   /* 多个状态之间 */
        @keyframes dong {
            0%{
                width: 300px;
                background-color: pink;
            }
            20%{
                width: 300px;
                background-color: blue;
            }
            100%{
                width: 400px;
                background-image: linear-gradient(gold,red);
            }
        }
    </style>
```

•   动画属性（空格隔开）

•   目标：使用animation相关属性控制动画执行过程

•   注意

1.动画名称和动画时长必须赋值

2.取值不分先后顺序

3.如果有2个时间值，第一个时间表示动画时长，第二个时间表示延迟时间

|            属性             |    作用     |                  取值                   |
| :-----------------------: | :-------: | :-----------------------------------: |
|      animation-name       |   动画名称    |                                       |
|    animation-duration     |   动画时长    |                                       |
|      animation-delay      |   延迟时间    |                                       |
|    animation-fill-mode    | 动画执行完毕时状态 | forwards：最后一帧状态  backwards：第一帧状态(默认值) |
| animation-timing-function |   速度曲线    |            steps(数字)：逐帧动画             |
| animation-iteration-count |   重复次数    |             infinite为无限循环             |
|    animation-direction    |  动画执行方向   |             alternate为反向              |
|   animation-play-state    |   暂停动画    |        paused为暂停，通常配合:hover使用         |

```html
div{
            width: 200px;
            height: 200px;
            background-color: pink;
            /* 动画的名称 */
            /* animation-name: run; */
            /* 动画的执行时间 */
            /* animation-duration: 2s; */
            /* 动画延迟执行时间 */
            /* animation-delay: 1s; */
            /* 执行完毕时的状态 */
            /* animation-fill-mode: forwards; */
            /* 步长 帧数 */
            /* animation-timing-function: steps(3); */
            /* 重复次数 */
            /* animation-iteration-count: infinite; */
            /* 反向执行 */
            /* animation-direction: alternate; */

            /* animation: run 2s linear 1s infinite alternate ; */
            animation: run 2s linear infinite alternate;
        }

```





## 07-逐帧动画

•   目标：使用steps实现逐帧动画

•   逐帧动画：帧动画。开发中，一般配合精灵图实现动画效果。

​	animation-timing-function:steps(N)；

​	将动画过程等分成N份

| 属性                        | 作用        | 取值                                    |
| ------------------------- | --------- | ------------------------------------- |
| animation-name            | 动画名称      |                                       |
| animation-duration        | 动画时长      |                                       |
| animation-delay           | 延迟时间      |                                       |
| animation-fill-mode       | 动画执行完毕时状态 | forwards：最后一帧状态  backwards：第一帧状态(默认值) |
| animation-timing-function | 速度曲线      | steps(数字)：逐帧动画                        |
| animation-iteration-count | 重复次数      | infinite为无限循环                         |
| animation-direction       | 动画执行方向    | alternate为反向                          |
| animation-play-state      | 暂停动画      | paused为暂停，通常配合:hover使用                |

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        div{
            width: 140px;
            height: 140px;
            background:  url(./img/bg.png);
            animation: run 1s steps(12) forwards;
        }

        @keyframes run {
            from{
                background-position: 0 0;
                transform: translateX(0);
            }
            to{
                background-position: -1680px 0;
                transform: translateX(1000px);
            }
        }
        p{
            width: 130px;
            height: 296px;
            background:  url(./img/警察.jpeg);
            animation: police 1s steps(8) forwards;
        }

        @keyframes police {
            from{
                background-position: 0 0;
                transform: translateX(0);
            }
            to{
                background-position: -1040px 0;
                transform: translateX(1000px);
            }
        }
    </style>
```



## 08-补间动画

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        div{
            width: 600px;
            height: 120px;
            border: 3px solid gray;
            margin: 100px auto;
            overflow: hidden;
        }
        li{
            width: 200px;
            height: 120px;
            list-style: none;
            float: left;
        }
        ul{
            width: 2000px;
            height: 120px;
            animation: move 3s linear infinite;
        }
        img{
            width: 100%;
            height: 100%;
        }
        @keyframes move{
            to{
                transform: translateX(-1400px)
            }
        }
        div:hover ul{
            animation-play-state: paused;
        }
    </style>
```



## 09-轮播图

```html
 <style>
        *{
            margin: 0;
            padding: 0;
        }
        div{
            width: 200px;
            height: 120px;
            border: 3px solid gray;
            margin: 200px auto;
            overflow: hidden;
        }
        ul{
            width: 1400px;
            height: 120px;
            animation: move 10s steps(7) infinite;
        }
        li{
            list-style: none;
            width: 200px;
            height: 120px;
            float: left;
        }
        img{
            width: 100%;
            height: 100%;
        }
        @keyframes move {
            to{
                transform: translateX(-1400px);
            }
        }
        div:hover>ul{
            animation-play-state: paused;
        }
    </style>
```



## 10-多列/分栏/瀑布流布局

•   添加在父元素上的

1、column-count：分栏的个数

2、column-width：分栏的宽度

3、column-gap：分栏的间距

4、column-rule：分栏的边框

•   写在子元素上的

1、column-span：all/1(默认)  合并分栏 

2、break-inside：定义页面、列或区域发生中断时候的元素该如何表现

  break-inside: auto;元素可以中断。

  break-inside:avoid;元素不能中断。

```html
  <style>
        ul{
            margin: 100 auto;
            width: 500px;
            height: 300px;
            list-style: none;
            /* 分栏的间距 */
            column-gap: 20px;
            /* 分栏的个数 */
            column-count:2 ;
            /* 分栏的宽度 */
            column-width: 100px;
            /* 分栏的边框 */
            column-rule: 1px;
        }

    </style>
```

```html
瀑布流布局

<style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            width: 400px;
            background-color: pink;
            margin: auto;
            list-style: none;
            /* 分栏数 */
            column-count: 3;
            /* column-width: 200px; */
            /* column-gap: 0; */
            column-rule: 3px dashed red;
        }
        li{
            background-color: orange;
        }
    </style>
```

# 移动端

图片居中

```html
.qu{
            display: flex;
            flex-direction: column;
           
            p:nth-of-type(1){
                font-size: 4vw;
                margin-bottom: 4.8vw;
                margin-top: 3.73vw;上边距别给父元素加，会被挤下来
            }
            p:nth-of-type(2){
                font-size: 3.2vw;
                color: #B4B4B4 ;
            }

        }



<div class="qu">
                <p>
                    趣味识地图―欢乐游戏中认识世界地图,亲子互动不可错过
                </p>
                <p class="iconfont icon-date">
                    2016.11.02-2016.11.0509: 30-18: 00
                </p>
            </div>
```

溢出的不占位

# day12-03.01

## 01-移动端介绍

•   PC端网页和移动端网页的有什么不同？

1.PC屏幕大，网页固定版心

2.手机屏幕小， 网页宽度多数为100%

•   屏幕尺寸：指的是屏幕对角线的长度，一般用英寸来度量

•   dpr是什么

1.设备像素比DPR(devicePixelRatio)是默认缩放为100%的情况下，设备像素和CSS像素的比值

2.DPR =设备像素（物理像素） /	CSS像素(某一方向上)

•   移动端页面书写

1、设备像素(deviceindependent pixels): 设备屏幕的物理像素，任何设备的物理像素的数量都是固定的

2、CSS像素(CSSpixels): 又称为逻辑像素，是为web开发者创造的，在CSS和javascript中使用的一个抽象的层

•   视觉视口（visualviewport）

视觉视口是用户当前看到的区域，用户可以通过缩放操作视觉视口，同时不会影响布局视口。

•   理想视口（idealviewport）

移动设备默认的viewport是布局视口（layoutviewport），但在进行移动设备网站的开发时，我们需要的是理想视口（ideal viewport）。

<meta
name="viewport"content="width=device-width,initial-scale=1,minimumscale=1,maximum-scale=1,user-scalable=no"/>

•   meta设置解析

1.maximum-scale=1.0  定义最大放大比例

2.minimum-scale=1.0  定义最小缩小比例

3.user-scalable=no  定义是否允许用户手动缩放页面，默认为yes

•   注意点：

1.viewport标签只对移动端浏览器有效，对 PC 端浏览器是无效的

2.单独设置initial-scale 或 width 都会有兼容性问题（横竖屏不分），所以设置布局视口为理想视口的最佳方法是同时设置这两个属性

3.即使设置了user-scalable = no，在 Android Chrome 浏览器中也可以强制启用手动缩放

## 02-flex

•   目标： 能够使用Flex布局模型灵活、快速的开发网页

•   作用:

1.基于Flex精确灵活控制块级盒子的布局方式，避免浮动布局中脱离文档流现象发生。

2.Flex布局非常适合结构化布局

•   设置方式：父元素添加display: flex，子元素可以自动的挤压或拉伸

•   组成部分 ：弹性容器，弹性盒子，主轴侧轴/交叉轴

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            width: 100%;
            height: 100px;
            background-color: pink;
            display: flex;
            justify-content: space-between;
        }
        li{
            list-style: none;
            /* float: left; */
            background-color: yellow;
            width: 100px;
            height: 100px;
            text-align: center;
            line-height: 100px;
            /* margin-right: 37.5px; */
        }
        /* ul li:nth-of-type(3){
            margin-right: 0;
        } */
    </style>
```



## 03-flex属性

•   目标：使用justify-content调节元素在主轴的对齐方式

1.不脱离标准流

2.父级添加display：flex的时候 弹性盒子横着排列

3.父级有高度，子集默认高度沾满

4.弹性盒子默认沿着主轴排列的

```html

```

## 04-主轴对齐方式	justify-content:center;

•   目标：使用justify-content调节元素在主轴的对齐方式

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        .box{
            height: 100px;
            background-color: green;
            display: flex;
            /* 默认 且子集全都紧靠一块*/
            justify-content: flex-start;
            /* 重点开始依次排列 整体偏移至右侧 且子集全都紧靠一块*/
            justify-content: flex-end;
            /* 子集整体居中 且子集全都紧靠一块*/
            justify-content: center;
            /* 眼主轴排列并且间距均匀加在盒子两侧 子集左右两边都有间距*/
            justify-content: space-around;
            /* 子集与子集之间的间距相等 最左和最右紧靠容器*/
            justify-content: space-between;
            /* 子集与子集之间，子集与容器之间间距都相等 */
            justify-content: space-evenly;
        }
        .son{
             width: 50px;
            /*height: 100px; */
            background-color: pink;
            text-align: center;
            line-height: 100px;
        }
       
    </style>
```



## 05-侧轴对齐方式	align-items：；

•   目标：使用align-items调节元素在侧轴的对齐方式

➢  修改侧轴对齐方式属性:

​	align-items（添加到弹性容器）

​	align-self：控制某个弹性盒子在侧轴的对齐方式（添加到弹性盒子)

```html
 <style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            height: 500px;
            background-color: pink;
            list-style: none;
            display: flex;
            /* 侧轴终点位置对齐 */
            /* align-items: flex-end; */
            /* 侧轴中间对齐 */
            align-items: center;
        }
        li{
            width: 80px;
            /* height: 80px; */
            background-color: green;
        }
    </style>
```

## 06-主轴方向	flex-direction：；

•   目标：使用flex-direction改变元素排列方向

•   主轴默认是水平方向, 侧轴默认是垂直方向

•   修改主轴方向属性:flex-direction

| 属性值            | 作用         |
| -------------- | ---------- |
| row            | 行, 水平(默认值) |
| column         | * 列, 垂直    |
| row-reverse    | 行, 从右向左    |
| column-reverse | 列, 从下向上    |

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        div{
            width: 200px;
            height: 200px;
            background-color: pink;
            display: flex;
            
            /* 改变主轴方向  */
            /* flex-direction: column; */
            /* flex-direction: row-reverse; */
            /* flex-direction: column-reverse; */
            /* align-items: center;
            justify-content: center; */
        }
        .icon-tianmao4{
            font-size: 30px;
        }
        div :nth-child(2){
            font-size: 20px;
            font-weight: 700;
        }
    </style>
</head>
<body>
    <div>
        <span class="iconfont icon-tianmao4"></span>
        <span>天猫商城</span>
    </div>
</body>
```

水平垂直居中

```html
<style>
        div{
            width: 200px;
            height: 200px;
            background-color: pink;

            display: flex;
            justify-content: center;水平
            align-items: center;垂直
            
        }
        span{
            width: 100px;
            height: 100px;
            background-color: green;
        }
    </style>
```



## **07**-伸缩比		flex:数字；

•   目标：使用flex属性修改弹性盒子伸缩比

​	给父级加上display:flex;	子集加上flex;数字；

•   注意 : 将父盒子剩余尺寸分成几份加上

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            height: 100px;
            background-color: pink;
            list-style: none;
            display: flex;
        }
        ul :nth-child(1){
            background-color: red;
            /* flex: 1; */
        }
        ul :nth-child(2){
            background-color: green;
            /* flex: 1; */
            flex: 1;
        }
        ul :nth-child(3){
            background-color: blue;
            flex: 1;
        }
    </style>
```

## 08-弹性盒子换行 flex-wrap:wrap;

•   目标：使用flex-wrap实现弹性盒子多行排列效果

•   弹性盒子换行显示 :flex-wrap:wrap;

➢  调整行对齐方式 ：align-content

| 属性值           | 作用                             |
| ------------- | ------------------------------ |
| flex-start    | 默认值, 起点开始依次排列                  |
| flex-end      | 终点开始依次排列                       |
| center        | 沿侧轴居中排列                        |
| space-around  | 弹性盒子沿侧轴均匀排列, 空白间距均分在每行弹性盒子上下两侧 |
| space-between | 弹性盒子沿侧轴均匀排列, 空白间距均分在相邻的每行盒子之间  |

```html
<style>
  *{
    margin:0;
    padding:0;
  }
  ul{
            height: 500px;
            background-color: pink;
            list-style: none;
            display: flex;
            flex-wrap: wrap;
            /* 从起点位置开始排列 侧轴的起点*/
            align-content: flex-start;
            /* 侧轴的终点位置 */
            align-content:flex-end;
            /* 侧轴的中间位置 */
            align-content: center;
            /* 行的上下间距相等，行与行之间是行与容器之间间距的2倍 */
            align-content: space-around;
            /* 行与行之间的间距相等 行与容器之间的间距为o */
            align-content: space-between;
            /* 行与行之间，行与容器之间间距相等 */
            align-content: space-evenly;
            justify-content: space-evenly;
        }
        li{
            width: 100px;
            height: 100px;
            background-color: aqua;
            /* margin-bottom: 5px; */
        }
    </style>
```

## 09-移动端项目前置

•   底部和头部不用再加固定定位

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        body,html{
            width: 100%;
            height: 100%;
        }
        body{
            display: flex;
            flex-direction: column;
        }
        header{
            height: 50px;
            background-color: pink;
        }
        section{
            background-color: blue;
            flex: 1;
        }
        footer{
            height: 50px;
            background-color: green;
        }
    </style>
</head>
<body>
    <header>头部</header>
    <section>主体</section>
    <footer>底部</footer>
</body>
```

# day13-03.02

## 01-rem适配

•   目标：能够使用rem单位设置网页元素的尺寸

➢  rem单位

​	相对单位

​	rem单位是相对于HTML标签的字号计算结果	1rem=1HTML字号大小

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        html{
            font-size: 20px;
        }
        div{
            /* 1rem默认16px html设置font-size是多少rem就是多少 */
            width: 2rem;
            height: 2rem;
            margin: auto;
            background-color: aqua;
        }
    </style>
```

➢  px、em、rem的区别

1.px是固定的像素，一旦设置了就无法因为适应页面大小而改变。

2.em和rem相对于px更具有灵活性，他们是相对长度单位，意思是长度不是定死了的，更适用于响应式布局。

3.em是相对于其父元素来设置字体大小的，一般都是以<body>的“font-size”为基准。这样就会存在一个问题，进行任何元素设置，都有可能需要知道他父元素的大小。而rem是相对于根元素<html>，这样就意味着，我们只需要在根元素确定一个参考值。

总之em相对于父元素，rem相对于根元素。

## 02-rem媒体查询

•   目标：能够使用媒体查询设置差异化CSS样式

```html
@media (width:414px) {
            html{
                font-size: 20px;
            }
        } 
```

## 03-rem设计网页

•   目标：能够使用rem单位设置网页元素的尺寸

•   目前rem布局方案中，将网页等分成10份， HTML标签的字号为视口宽度的 1/10

​	例如：宽度375px，1rem为其1/10即37.5px

•   目标：使用flexible js配合rem实现在不同宽度的设备中，网页元素尺寸等比缩放效果



```html
<style>
div{
            width: 2rem;
            height: 2rem;
            background-color: aqua;
        }
    </style>
<body>
    <script src="./js/flexible.js"></script>
    <div>

    </div>
</body>
```

##  04-less

•   目标：使用Less语法快速编译生成CSS代码

•   作用：less文件保存自动生成css文件

➢  注释：

​	单行注释

​		语法：// 注释内容

​		快捷键：ctrl + /

​	块注释

​		语法：/* 注释内容 */

​		快捷键： shift+ alt+ A

```less
// 单行注释 ctrl + /

/* 块注释  shift + alt + A*/
```

•   目标：使用Less运算写法完成px单位到rem单位的转换

➢  运算：

1.加、减、乘直接书写计算表达式

2.除法需要添加 小括号里面

3.表达式存在多个单位以第一个单位为准

```less
.box{
    width: 100px+100px;
    width: 100px-50px;
    width: 100px*12px;
    /* 除法需要添加小括号  px单位到rem单位的转换*/
    width: (100/37.5rem);
}
```

➢  目标：能够使用Less嵌套写法生成后代选择器

```less
.father{
    width: 500px;
    height: 500px;
    background-color: pink;
    // 这个区域是我写的头部的左边，并且上面有一个字体图标
    .box1{
        width: 300px;
        height: 300px;
        background-color: green;
        .son{
            width: 100px;
            height: 100px;
            background-color: orange;
            display: none;
        }
        &:hover .son{
            display: block;
        }
    }
    /* .box1:hover .son{
        display: block;
    } */
    .box2{
        width: 300px;
        height: 300px;
        background-color: blue;
        &>:nth-child(1){
            width: 100px;
            height: 100px;
            background-color: aqua;
        }
        &>:nth-child(1)+div{
            width: 100px;
            height: 100px;
            background-color: purple;
        }
        &>:nth-child(3){
            background-color: brown;
        }
    }
}
```

➢  目标：能够使用Less变量设置属性值

•   方法： 把颜色提前存储到一个容器，设置属性值为这个容器命名

•   变量：存储数据，方便使用和修改。

•   语法：

​	定义变量：@变量名: ;

​	使用变量：CSS属性：@变量名;

```less
// 1. 定义. 2.使用
@colors:green;

@size:37.5rem;

div{
    width: (68 / @size);
    height: (29 / @size);
    color: @colors;
}

p{
    color: @colors;
}

span{
    background-color: @colors;
}
```

➢ 目标：能够使用Less导入写法引用其他Less文件

导入: @import “文件路径”;

```less
@import "./02-注释.less";

@import "./03-计算";
```

➢ 目标：使用Less语法导出CSS文件

```less
//out:./css/
//out:./css/index1
```

方法一：配置EasyLess插件， 实现所有Less有相同的导出路径	“out”:"./"

方法二：控制当前Less文件导出路径	Less文件第一行添加如下代码, 注意如果是文件夹名称后面添加 /

•   禁止导出： 在less文件第一行添加: // out: false

```less
//out:false
```

# day15-03.03

## 01-单行溢出省略号

•   要实现单行文本溢出时产生省略号的效果还需定义：

1、容器宽度：width：value；

2、强制文本在一行内显示:white-space：nowrap;

3、溢出内容为隐藏：overflow：hidden；

4、溢出文本显示省略号：text-overflow：ellipsis;

```html
<style>
        div{
            margin: 200px auto;
            width: 200px;
            height: 100px;
            /* 强制文本在一行内显示 */
            white-space: nowrap;
            /* 溢出内容为隐藏 */
            overflow: hidden;
            /* 溢出文本显示省略号 */
            text-overflow: ellipsis;
        }
    </style>
```

## 02-多行溢出省略

•   要实现多行文本溢出时产生省略号的效果还需定义：

1、display:-webkit-box------------将对象作为弹性伸缩盒子模型显示 

2、-webkit-box-orient:vertical----设置或检索伸缩盒对象的子元素的排列方式 。

3、-webkit-line-clamp:2----用于显示的行数

4、overflow:hidden\----溢出文本显示省略号

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        div{
            width: 200px;
            /* 转成弹性伸缩盒子 */
            display: -webkit-box ;
            /* 限定文字排列方式 */
            -webkit-box-orient: vertical;
            /* 显示行数 */
            -webkit-line-clamp: 2;
            /* 不用加上overflow:hidden; 可以设置行高；盒子没设高度时，高度由内容撑开*/
        }
    </style>
```

## 03-flex 元素的收缩	flex-shrink  

取值：1  默认压缩

取值：0  不被压缩

注意：给子元素弹性盒子添加

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        /* 取消滚动条 */
        ::-webkit-scrollbar{
            display: none;
        }
        ul{
            width: 100%;
            height: 50px;
            list-style: none;
            display: flex;
            background-color: pink;
        }
        li{
            /* width: 80px; */
            height: 50px;
            text-align: center;
            line-height: 50px;
            flex-shrink: 0;不被压缩
            margin: 0 10px;
           
        }
        li:hover{
            color: aqua;
            border-bottom: solid 2px gold;
        }
    </style>
```

## 04-vw/vh

•   目标：能够使用vw单位设置网页元素的尺寸

•   相对单位

vw：viewport width

1vw = 1/100视口宽度

lvh：viewport height

1vh=1/100视口高度

## 05-vw适配原理

•   目标：实现在不同宽度的设备中，网页元素尺寸等比缩放效果

```less
// out:./
*{
    margin: 0;
    padding: 0;
}
@vw: 3.75vw;
@vh: 6.67vh;
div{
    width: (68 / @vw);
    height: (28 / @vw);
    background-color: aqua;
}
p{
    width: (68 / @vh);
    height: (28 / @vh);
    background-color: gold;
}
```

全面屏手机高度更高，如果vw和vh混用，会造成效果变形

```less
p{
    width: (68 / @vh);
    height: (28 / @vh);
    background-color: gold;
}

i{
    display: block;
    width: (68 / @vw);
    height: (28 / @vh);
    background-color: blue;
}

```

# day16-03.06

## 01-vmin vmax

vmin 可视窗口长度较短的那边

vmax 可视窗口长度较长的那边

解决移动端横屏问题

## 02-单位

​	px    像素单位 固定单位绝对单位

​        %     %单位相对单位，相对最近的父级进行参照判断

​        em    相对单位，参照内容所在标签的font-size设置的值，默认是16px 默认字号大小是16px

​        pt    12pt = 16px

​        rem   相对单位，参照html根元素的字号大小，html{font-size:...},默认根字号大小为16px

​        vw    相对单位，参照视口宽度进行判断，1vw=1/100视口宽度

​        vh    相对单位，参照时候高度进行判断，1vh=1/100视口高度

​        vmin  相对单位，参照视口最小的那一边进行判断，正常情况下跟vw一致

​        vmax  相对单位，参照视口最小的那一边进行判断，正常情况下跟vh一致

## 03-rem单位的使用

•   快捷键;alt+z	px-rem转换（二倍图）

# day17-03.07

## 01-设置网格布局

•   网格布局（Grid）它将网页划分成一个个网格，可以任意组合不同的网格，做出各种各样的布局

➢   grid布局相关概念

1.采用网格布局的区域，称为"容器"（container）。

2.容器内部采用网格定位的子元素，称为"项目"（item）。

3.注意：项目只能是容器的顶层子元素，不包含项目的子元素。Grid布局只对项目生效。

```less
ul{
            width: 300px;
            height: 300px;
            border: 3px solid gray;
            /* overflow: hidden; */
            /* 父级转换成网格容器 */
            display: grid;
            /* 
                特点：
                    1.子集高度默认拉伸占满父级的高度
                    2.子集无论是什么显示模式都竖着排列，并且宽度拉伸占满父级的宽度
                    3.默认产生网格线
            */

            /* 行内网格 */
            /* display: inline-grid; */
        }
```



## 02-设置网格的行高和列宽	grid-template-columns	grid-template-rows

1、display：grid；  display：inline-grid；指定一个容器采用网格布局

2、grid-template-columns属性   设置每列的列宽,参数的个数决定是几列

3、grid-template-rows属性     定义每一行的行高

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            width: 300px;
            height: 300px;
            list-style: none;
            display: grid;
            margin: auto;
            border: 3px solid aqua;
            /* 具体数值 */
            /* 3列 */
            grid-template-columns: 100px 100px 100px;
            /* 4列 会超出，实际做项目的时候注意宽度*/
            grid-template-columns: 100px 100px 100px 100px;
            /* 重复执行 */
            /* 重复执行3次两列100px 共六列 */
            grid-template-columns: repeat(3,100px 100px);
            /* 如果子集个数小于设置的列数,网格线会存在，不影响整体布局*/
            /* % */
            grid-template-columns: 10% 20%;
            /* 百分比可以和具体数值混用 */
            grid-template-columns: 10% 100px;
            grid-template-columns: repeat(2,10% 100px);
            /* 片段 */
            grid-template-columns: 1fr 1fr 2fr;
            grid-template-columns: repeat(2,1fr);




            /* 行高 */
            /* 具体数值 */
            grid-template-rows: 50px 50px;
            /* % */
            grid-template-rows: 10% 20%;
            /* 片段 */
            /* 在设置行高的时候，用fr片段进行书写repet(当,1fr),逻辑为提出除前三个之外元素剩余空间均 */
            grid-template-rows: repeat(3,1fr);
        }
        li{
            background-color: gold;
        }
    </style>
```



## 03-设置网格的间距	grid-gap

•    grid-gap属性是grid-column-gap和grid-row-gap的合并简写 设列间距和行间距  外边距也可调整

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            width: 300px;
            height: 300px;
            list-style: none;
            display: grid;
            margin: auto;
            border: 3px solid black;
            grid-template-columns: repeat(3,1fr);
            grid-template-rows: repeat(3,1fr);

            /* 设置列间距 */
            /* 如果列宽或者行宽设的具体数值100px间距会多出来 撑大盒子
            grid-template-columns: repeat(3,100px);
            grid-template-rows: repeat(3,100px);
            */
            grid-column-gap: 10px;
            /* 设置行间距 */
            grid-row-gap: 10px;
            /* 连写，第一个代表行间距 第二个为列间距 */
            grid-gap: 10px 20px;
        }
        li{
            background-color: aqua;
        }
    </style>
```



## 04-设置子元素位置	place-items

•    place-items：place-items属性是justify-items属性和align-items属性的合并简写形式，设置单元格内容在网格内的水平垂直对齐方式。

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            width: 300px;
            height: 300px;
            list-style: none;
            display: grid;
            margin: auto;
            border: 3px solid black;
            grid-template-columns: repeat(3,100px);
            grid-template-rows: repeat(3,100px);
            /* justify-items: stretch;默认拉伸 */
           /* justify-items: start;水平左对齐 */
            /* justify-items: center;水平居中对齐 */
            /* justify-items: end;水平右对齐 */

            /* align-items: stretch;默认拉伸占满 */
            /* align-items: start;水平上对齐 */
            /* align-items:center;垂直中间对齐 */
            /* align-items: end;垂直下对齐 */

            /* 第一个取值代表垂直方向 第二个代表水平方向 */
            place-items: center end;中右
            place-items: center start;中左
            place-items: center center;居中

        }
        li{
            background-color:aqua ;
        }
    </style>
```

## 05-设置网格整体在容器中移动	 place-content

•    place-content属性是justify-content属性和align-content属性的合并简写形式。设置整个内容区域在容器里面的水平和垂直位置。

```html
<style>
    *{
            margin: 0;
            padding: 0;
        }
        ul{
            width: 300px;
            height: 300px;
            list-style: none;
            display: grid;
            margin: auto;
            border: 3px solid black;
            grid-template-columns: repeat(3,80px);
            grid-template-rows: repeat(3,80px);

            /* justify-content: stretch拉伸默认*/
            /*justify-content: start;水平靠左对齐*/
            /*justify-content: center;水平居中对齐*/
            /*justify-content: end;水平靠右对齐*/
            /* justify-content: space-around;列与列之间的间距是列与容器之间间距的两倍*/
            /* justify-content: space-between;列与列之间的间距相等，列与容器之间的间距为零*/
            /* justify-content: space-evenly;列与列之间的间距，列与容器之间的间距均相等*/


            /* align-content:stretch; 默认拉伸*/
            /* align-content: start;垂直靠上对齐 */
            /* align-content: center;垂直居中对齐 */
            /* align-content: end;垂直靠下对齐 */
            /* align-content: space-around;行与行之间的间距是行与容器之间间距的两倍*/
            /* align-content: space-between;行与行之间的间距相等，行与容器之间的间距为零*/
            /* align-content: space-evenly;行与行之间的间距，行与容器之间的间距均相等*/

            /* 第一个代表垂直方向，第二个水平方向
            默认左上角 */
            /* place-content: center end;中右 */
            /* place-content: center;中 */
            /* place-content: end;右下 */
            /* place-content: start flex-end;右上，不建议 */
        }

        li{
            background-color: aqua;
        }
    </style>
```



## 06-划分区域	grid-template-areas

•    grid-template-areas 属性  网格布局允许指定"区域"（area）

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            width: 300px;
            height: 300px;
            list-style: none;
            display: grid;
            margin: auto;
            border: 3px solid black;
            grid-template-columns: repeat(3,80px);
            grid-template-rows: repeat(3,80px);
            grid-template-areas: 
            
            'a b c'		可以是中文但不建议
            'd e f'
            'g h i'           
            ;
        }
        li{
            background-color: aqua;
        }

        
        /* 两个区域放在同一块区域时，看标签结构谁在后显示谁 */
        ul>li:nth-of-type(1){
            grid-area: i;
        }
        ul>li:nth-of-type(3){
            grid-area: i;
        }
    </style>
```

## 07-合并网格	grid-area:;

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            width: 300px;
            height: 300px;
            list-style: none;
            display: grid;
            margin: auto;
            border: 3px solid black;
            grid-template-columns: repeat(3,80px);
            grid-template-rows: repeat(3,80px);
            grid-template-areas: 
            
            'a a a'
            'd e e'
            'd e e'           
            ;
        }
        li{
            background-color: aqua;
        }

        /* 左上原则，不用的注释掉 */
        /* 合并1 2 3 */
        ul>li:nth-of-type(1){
            grid-area: a;
        }
        /* 合并4 7 */
        ul>li:nth-of-type(2){
            grid-area: d;
        }
        /* 合并5 6 8 9 */
        ul>li:nth-of-type(3){
            grid-area: e;
        }
    </style>
</head>
<body>
    <ul>
        <li>1</li>
        <!-- <li>2</li> -->
        <!-- <li>3</li> -->
        <li>4</li>
        <li>5</li>
        <!-- <li>6</li> -->
        <!-- <li>7</li> -->
        <!-- <li>8</li> -->
        <!-- <li>9</li> -->
    </ul>
</body>
```

## 08-直接用线合并	grid-area: 1/1/2/4;

•    适用于多个方块

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            width: 300px;
            height: 300px;
            list-style: none;
            display: grid;
            margin: auto;
            border: 3px solid black;
            grid-template-columns: repeat(3,80px);
            grid-template-rows: repeat(3,80px);
        }
        li{
            background-color: aqua;
        }
        /* 左上原则，不用的注释掉 */
        /* 行的开始/列的开始/行的结束/列的结束 */
        /* 合并1 2 3 */
        ul>li:nth-of-type(1){
            grid-area: 1/1/2/4;
        }
        /* 合并4 7 */
        ul>li:nth-of-type(2){
            grid-area: 2/1/4/2;
        }
        /* 合并5 6 8 9 */
        ul>li:nth-of-type(3){
            grid-area: 2/2/4/4;
        }
    </style>
</head>
<body>
    <ul>
        <li>1</li>
        <!-- <li>2</li> -->
        <!-- <li>3</li> -->
        <li>4</li>
        <li>5</li>
        <!-- <li>6</li> -->
        <!-- <li>7</li> -->
        <!-- <li>8</li> -->
        <!-- <li>9</li> -->
    </ul>
</body>
```

## 09-单个网格设置	place-self 

place-self  设置项目自己的对齐方式

place-self是justify-self和align-self的简写

place-self：start | end | center | stretch；

```html
 <style>
        *{
            margin: 0;
            padding: 0;
        }
        ul{
            width: 300px;
            height: 300px;
            list-style: none;
            display: grid;
            margin: auto;
            border: 3px solid black;
            grid-template-columns: repeat(3,80px);
            grid-template-rows: repeat(3,80px);
        }
        li{
            background-color: aqua;
        }
        li:nth-of-type(1){
            /* 宽高由内容撑开 */
            /* justify-self: start;水平靠左对齐 */
            /* justify-self: center;水平居中对齐*/
            /* justify-self: end;水平靠右对齐*/


            /* align-self: start;垂直靠上对齐*/
            /* align-self: center;垂直居中对齐*/
            /* align-self: end;垂直靠下对齐*/


            /* 第一个代表垂直方向，第二个水平方向 */
            /* place-self: center;垂直正居中 */
          /* place-self: stretch;默认拉伸占满 */
            place-self: start center;上中

        }

    </style>
```

# day18-03.08

## 01-锚点跳转

•    命名锚点的作用：在同一页面内的不同位置进行跳转。

```html
<style>
        div{
            width: 200px;
            height: 200px;
            border: 1px solid aqua;
        }

        h1{
            width: 200px;
            height: 200px;
            background-color: pink;
            position: fixed;
            right: 200px;
            top: 10px;
        }
    </style>
</head>
<body>
    <div id="a1">
        <p>第一章</p>
    </div>
    <div id="a2">
        <p>第二章</p>
    </div>
    <div id="a3">
        <p>第三章</p>
    </div>
    <div id="a4">
        <p>第一章</p>
    </div>
    <div id="a5">
        <p>第一章</p>
    </div>
    <div id="a6">
        <p>第一章</p>
    </div>
    
    <h1>
        <a href="#a1">1</a>
        <a href="#a2">2</a>
        <a href="#a3">3</a>
        <a href="#a4">4</a>
        <a href="#a5">5</a>
        <a href="#a6">6</a>
    </h1>
</body>
```



## 02-二级菜单

•    无序列表结构进行多层嵌套

•    配合:hover，过渡transition:all 3slinear实现简易的二级菜单效果，具体实现功能，需要配合js

•    实现缓慢的效果==不能使用display:none/block===不参与过渡

```html
<style>
        *{
            margin: 0;
            padding: 0;
        }
        nav{
            background-color: aqua;
            height: 50px;
        }
        .dao{
            width: 600px;
            height: 50px;
            margin: auto;
            background-color: gold;
            list-style: none;
            display: flex;
            
        }
        .dao>li{
            width: 200px;
            height: 50px;
            background-color: pink;
            text-align: center;
            line-height: 50px;
        }
        .dao>li>ul{
            list-style: none;
            margin: auto;
            width: 150px;
            height: 50px;
            background-color: burlywood;
            /* 用display不能用过渡transition
            display: none; */
            height: 0;
            transition: all linear 1s;
            overflow: hidden;
        }
        .dao>li:nth-of-type(1):hover ul{
            /* display: block; */
            height: 150px;
        }
    </style>
</head>
<body>
    <nav>
        <ul class="dao">
            <li>导航1
                <ul>
                    <!-- 小黑点变成空心圆 -->
                    <li>子导航1</li>
                    <li>子导航2</li>
                    <li>子导航3</li>
                </ul>
            </li>
            <li>导航2</li>
            <li>导航3</li>
        </ul>
    </nav>
</body>
```



## 03-响应式页面	媒体查询

➢   关键词：and  和	only  仅一个	not   非

➢   媒体类型：媒体是用来区分设备类型的，如屏幕设备、打印设备等，其中手机、电脑、平板都属于屏幕设备

| 类型名称  | 值      | 描述           |
| ----- | ------ | ------------ |
| 屏幕    | screen | 带屏幕的设备       |
| 打印预览  | print  | 打印预览模式       |
| 阅读器   | speech | 屏幕阅读模式       |
| 不区分类型 | all    | 默认值，包括以上3种情形 |

➢   媒体特征：媒体特性主要用来描述媒体类型的具体特征，如当前屏幕的宽高、分辨率、横屏或竖屏等。

| 特性名称    | 属性                   | 值                             |
| ------- | -------------------- | ----------------------------- |
| 视口的宽和高  | width、height         | 数值                            |
| 视口最大宽或高 | max-width、max-height | 数值                            |
| 视口最小宽或高 | min-width、min-height | 数值                            |
| 屏幕方向    | orientation          | portrait: 竖屏    landscape: 横屏 |

```less
/* 完整写法 */
        @media screen and (max-width:768px) {
            body{
                background-color: gold;
            }
            /* 和平常写样式一样 */
            h1{
                color: red;
                font-size: 20px;
                width: 100px;
                height: 50px;
                background-color: aqua;
            }
            div{
                background-color: gold;
            }
        }
        @media screen and (orientation:portrait) {
            h1{
                color: black;
            }
        }
```

➢   外链式CSS引入

```html

<!-- 
        视口宽度>=992px，网页背景色为粉色
        视口宽度>=1200px，网页背景色为绿色

     -->
     <link rel="stylesheet" href="./one.css" media="(min-width:992px)">
     <link rel="stylesheet" href="./two.css" media="(min-width:1200px)">
```

•    目标：能够根据设备宽度的变化，设置差异化样式

min-width（从小到大）

max-width（从大到小）

```html
<style>
        /* 视口宽度小于等于768px,网页背景色是粉色*/
        @media (max-width:768px) {
            body{
                background-color: pink;
            }
        }

        /* 视口宽度大于等于1200px，网页背景色是skyblue */
        @media (min-width:1200px) {
            body{
                background-color: skyblue;
            }
        }
    </style>
```

## 04-媒体查询书写顺序

```html
<style>
        /* 
        视口宽度>= 768px，网页背景色是粉色
        视口宽度>= 992px，网页背景色是绿色
        视口宽度>=1200px，网页背景色是skyblue

        当条件都是min-width的时候取值的书写顺序是由小到大

        */
         @media (min-width:768px) {
            body{
                background-color: pink;
            }
        }
        @media (min-width:992px) {
            body{
                background-color: blue;
            }
        }
        @media (min-width:1200px) {
            body{
                background-color: skyblue;
            }
        }

        /* 
        视口宽度<= 768px，网页背景色是粉色
        视口宽度<= 992px，网页背景色是绿色
        视口宽度<=1200px，网页背景色是skyblue

        
        当条件都是max-width的时候取值的书写顺序是由大到小 */
       
        
        @media (max-width:1200px) {
            body{
                background-color: skyblue;
            }
        }
        @media (max-width:992px) {
            body{
                background-color: blue;
            }
        }
        @media (max-width:768) {
            body{
                background-color: pink;
            }
        }
    </style>
```

## 05-隐藏

```html
 <style>
        *{
            margin: 0;
            padding: 0;
        }
        .box{
            width: 100%;
            height: 600px;
            background-color: pink;
            display: flex;
        }
        .left{
            width: 200px;
            height: 100%;
            background-color: blue;
        }
        .main{
            width: 900px;
            height: 300px;
            background-color: aqua;
        }
        @media (max-width:992px) {
            .left{
              /* 隐藏但是占位 */
                visibility: hidden;
                display: none;
            }
            .main{
                color: red;
            }
        }
    </style>
</head>
<body>
    <div class="box">
        <div class="left">
            left
        </div>
        <div class="main">
            宣布个事，我是帅哥.宣布个事，我是帅哥.宣布个事，我是帅哥
            宣布个事，我是帅哥.宣布个事，我是帅哥.宣布个事，我是帅哥
            宣布个事，我是帅哥.宣布个事，我是帅哥.宣布个事，我是帅哥
            宣布个事，我是帅哥.宣布个事，我是帅哥.宣布个事，我是帅哥
            宣布个事，我是帅哥.宣布个事，我是帅哥.宣布个事，我是帅哥
            宣布个事，我是帅哥.宣布个事，我是帅哥.宣布个事，我是帅哥
            宣布个事，我是帅哥
            宣布个事，我是帅哥
            宣布个事，我是帅哥
        </div>
    </div>
</body>
```

## 06-Bootstrap使用方法

•    目标：使用 BootStrap框架快速开发响应式网页

•    Bootstrap 是由 Twitter 公司开发维护的前端 UI框架，它提供了大量编写好的 CSS 样式，允许开发者结合一定HTML结构及JavaScript，快速编写功能完善的网页及常见交互效果。

•    中文官网: https://[www.bootcss.com/](http://www.bootcss.com/)

•    使用步骤

1. 引入： BootStrap提供的CSS代码
2. 调用类：使用BootStrap提供的样式

## 07-BootStrap栅格系统

•    目标：使用BootStrap栅格系统布局响应式网页

•    栅格化是指将整个网页的宽度分成若干等份

•    BootStrap3默认将网页分成12等份

•    .container是 Bootstrap 中专门提供的类名，所有应用该类名的盒子，默认已被指定宽度且居中。

•    .container-fluid也是 Bootstrap 中专门提供的类名，所有应用该类名的盒子，宽度均为 100%。

•    分别使用.row类名和 .col类名定义栅格布局的行和列。



•    注意:

1.container类自带间距15px;

2.row类自带间距-15px

|      | 超小屏幕    | 小屏幕     | 中等屏幕    | 大屏幕      |
| ---- | ------- | ------- | ------- | -------- |
| 响应断点 | <768px  | >=768px | >=992   | >=1200px |
| 别名   | xs      | sm      | md      | lg       |
| 容器宽度 | 100%    | 750px   | 970px   | 1170px   |
| 类前缀  | col-xs- | col-sm- | col-md- | col-lg-  |
| 列数   | 12      | 12      | 12      | 12       |
| 列间隙  | 30px    | 30px    | 30px    | 30px     |

```html
<link rel="stylesheet" href="./bootstrap-3.4-1.1-dist/css/bootstrap.min.css">
    <style>
        .container{
            height: 60px;
            background-color: aqua;
        }
        a{
            display: block;
        }
    </style>
</head>
<body>
    <div class="container">
        <a href="#" class="col-sm-12 col-md-6 col-lg-3">1</a>
        <a href="#" class="col-sm-12 col-md-6 col-lg-3">2</a>
        <a href="#" class="col-sm-12 col-md-6 col-lg-3">3</a>
        <a href="#" class="col-sm-12 col-md-6 col-lg-3">4</a>
    </div>
</body>
```

➢   全局css样式-表格

```html
<link rel="stylesheet" href="./bootstrap-3.4-1.1-dist/css/bootstrap.min.css">
    <style>

    </style>
</head>
<body>
    <!-- 先link,再从网页上看需要哪个样式，就给标签加类名，类名可以添加多个，一定要先加个table类名
        需要自己添加样式，需要注意权重 -->
    <table class="table table-bordered table-striped">
        <tr>
            <th>年龄</th>
            <th>性别</th>
            <th>爱好</th>
        </tr>
        <tr>
            <td>18岁</td>
            <td>男</td>
            <td>女</td>
        </tr>
        <tr>
            <td>18岁</td>
            <td>男</td>
            <td>女</td>
        </tr>
    </table>
</body>
```

