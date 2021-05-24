# 前端复习
根据技术胖前端学习路线复习.  
如图 前端学习路线.png 所示。 
![2021前端学习路线](https://newimg.jspang.com/web-router.png)  


## 1. HTML5+CSS3
### 1.1 HTML基本标签和属性
HTML 参考手册- (HTML5 标准)  
[按字母顺序排列](https://www.runoob.com/tags/html-reference.html)
### 1.2 H5新标签及属性
参考 [HTML5 新元素](https://www.runoob.com/html/html5-new-element.html)
#### 新增的语义化标签
一：结构标签（语义化标签）  
| 名称 | 描述 |
|  :----:  | :----  |
| section | section标签定义文档中的节（section、区段）。比如章节、页眉、页脚或文档中的其他部分。 |
| article | article标签装载显示一个独立的文章内容。还可以嵌套，则内层的artilce对外层的article标签有隶属的关系。例如，一个博客文章，可以用article显示，然后一些评论可以以article的形式嵌入其中。 |
|aside|标签内容之外与标签内容相关的辅助信息|
|header|header标签定义文档的页面组合，通常是一些引导和导航信息。|
|hgroup|hgroup标签用于对网页或区段的标题元素（h1-h6）进行组合。例如，在一个区段中你有连续的h系列的标签元素，则可以用hgroup将他们括起来。 |
|footer|页尾信息|
|nav|nav标签定义显示导航链接。|  
|figure|独立的单元，例如某个有图片与内容的新闻块。|
|time|time标签定义公历的时间（24 小时制）或日期，时间和时区偏移是可选的。该元素能够以机器可读的方式对日期和时间进行编码，这样， 举例说，用户代理能够把生日提醒或排定的事件添加到用户日程表中，搜索引擎也能够生成更智能的搜索结果。 |
|mark|mark标签定义带有记号的文本。|
|figure|figure标签规定独立的流内容（图像、图表、照片、代码等等）。figure 元素的内容应该与主内容相关，但如果被删除，则不应对文档流产生影响。|
|figcaption|figcaption 标签定义 figure 元素的标题（caption）。"figcaption" 元素应该被置于 "figure" 元素的第一个或最后一个子元素的位置。类似图名|

#### 二：新增表单type属性值
1.type="email"。必须输入邮件。  
2.type="url"。必须输入url地址。  
3.type="number"。必须输入数值。  
4.type="range"。必须输入一定范围内的数值。  
5.type="Date Pickers"。日期选择器。  
6.type="search"。搜索常规的文本域。  
7.type="color"。颜色。  
#### 三：媒体标签
1.video。视频  
2.audio。音频  
3.embed。嵌入内容（包括各种媒体），Midi、Wav、AU、MP3、Flash、AIFF等。  
4.source。source设置两份或多份源文件的音频播放器。浏览器应该选择它所支持的文件（如果有的话）  
5.track。诸如 video 元素之类的媒介规定外部文本轨道。用于规定字幕文件或其他包含文本的文件，当媒介播放时，这些文件是可见的。  

### 1.3 CSS基本样式
#### 1.3.1 选择器
参考 [CSS的四种基本选择器和四种高级选择器](https://blog.csdn.net/DYD850804/article/details/80997251?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control)  
1、标签选择器：选择器的名字代表html页面上的标签
```
<style type="text/css">
p{
    font-size:14px;
}
</style>

<body>
<p>css</p>
</body>
```
【总结】需要注意的是：  
（1）所有的标签，都可以是选择器。比如ul、li、label、dt、dl、input、div等。  
（2）无论这个标签藏的多深，一定能够被选择上。  
（3）选择的所有，而不是一个。  
2、ID选择器：规定用#来定义（名字自定义）
#### 1.3.2 盒子模型  
不同部分的说明：  
**Margin(外边距)** - 清除边框外的区域，外边距是透明的。  
**Border(边框)** - 围绕在内边距和内容外的边框。  
**Padding(内边距)** - 清除内容周围的区域，内边距是透明的。  
**Content(内容)** - 盒子的内容，显示文本和图像。  
![盒子模型](https://www.runoob.com/images/box-model.gif)  
#### 1.3.3 定位、浮动