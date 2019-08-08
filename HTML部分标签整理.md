# HTML文本，图片，超链接，表格标签及转义字符
## 文本标签

```
1. 标题标签：<h1></h1>~<h6></h6>
2. 段落标签：<p></p>
3. 换行标签：<br/>
4. 引用文本标签：<q></q> 
5. 段落缩进标签：<blockquote></blockquote>
7.粗体标签：<b > </b >,<strong></strong>——区别在于,否则是强调的，带一种“语义”的标签
8.斜体标签：<em></em>——带强调的，带一种“语义”
9.原样输出标签：<pre></pre>
10.上标标签：<sup></sup>——【x<sup>2</sup>:显示x的平方】
11.下表标签：<sub></sub>——【CO<sub>2</sub>:显示化学符号CO2】
12.行内标签：<span></span>——表单验证会使用此标签
13.快标签：<div></div>
```

14.滚动标签：< marquee > < /marquee>

属性：

*   behavior属性——滚动方式
```
*             alternate:来回滚动
*             scrooll:交替滚动
*             slide:沿着滚动的方向滚动一次
```
* scrollamount属性：滚动的速度

* direction属性:滚动的方向

* bgcolor属性：背景色【标签属性】
  例：

* ```
  <marquee behavior=" alternate"  direction="right"   scrollamount=“10”bgcolor=“green”> hello html!</marquee>
  ```



  15.无序列表标签：
```
属性：type——默认为dise[实心圆点]，可选circlre[空心圆点]，squaer[实心方块]
<ul>
    <li>列表内容1</li>
    <li>列表内容2</li>
    <li>列表内容3</li>
</ul>
```
16.有序列表标签：

```
属性：type——默认为123格式，可选为ABC或abc
<ol>
    <li>列表内容1</li>
    <li>列表内容2</li>
    <li>列表内容3</li>
</ol>
```
17.项目组织架构列表：

```
<dl>
    <dt>
        <dd>xxx</dd>
        <dd>yyy</dd>
        <dd>zzz</dd>
    </dt>
</dl>
```
## 图片标签：
<img>标签：

```
常用属性：src:加载图片文件地址（路径：相对路径）
width/height:指定图片的宽度和高度（px/宽高百分比）
alt:替代文本（图片链接失效时起作用）
title:鼠标悬浮在图片上的时候，提示文字
```
超链接标签：

<a>标签：

```
常用属性：
herf:url（统一资源定位符）
target:打开连接资源文件的方式
        默认为：_self：当前窗口直接打开
          可选：_blank：新建窗口打开
```
超链接的作用：
*   作为资源文件
*   作为锚连接使用
```
在同一页面下使用：
步骤：
1.打锚点（做标记）<a name = "锚点名称"></a>
2.创建跳转连接（跳到锚点位置）<a href="#锚点名称">执行跳转</a>
在不同页面下使用：
步骤：
1.在指定html页面中打锚点（做标记）<a name = "锚点名称"></a>
2.创建跳转连接（跳到锚点位置）<a href="连接url#锚点名称">执行跳转</a>
```

## 表格标签：

```
<table></table>
```

作用：网页布局
```
行标签：<tr></tr>
表头标签：<th></th>(自动加粗居中)
单元格标签：<td></td>
```
```
属性：
border：边框大小（px）
align：在浏览器中显示对齐方式
bgcolor：背景颜色
cellspacing：控制单元格和边框之间的空隙
```
```
应用：
合并行：rowspan="number"
列合并：cosspan="number"
```
## 转义字符：

```
空格：&nbsp;
版权所有：&copy;
注册商标：&reg;
```

空格：&nbsp;
版权所有：&copy;
注册商标：&reg;