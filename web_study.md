# markdown使用教程

```html
1. *斜体*，_斜体_    (快捷键Ctrl+I)
2. **粗体** 		  (快捷键Ctrl+B)
3. ***粗斜***			   
4. ~~删除线~~		 (快捷键Alt Shift+5)
5. <u>下划线</u>	 (快捷键Ctrl+U)
6. <center>居中</center>

标题：
1.# 一级标题
2.##二级标题
3.###三级标题

超链接：
[B站](https://www.bilibili.com "链接标题")
快捷键：Ctrl+K

列表：
1. * 无序列表
2. + 无序列表
3. - 无序列表
(数字句号空格)
1. 有序列表
2. 有序列表有序列表

引用：
*	引用列表
      >第一层
        >>第二层
       	 >>>第三层
       	
插入图片：
1.快捷键：ctrl+shift+i
2.行内式
![长泽雅美](https://gitee.com/xsyzer/image_01/raw/master/img/20200416131451.png)
3.参考式
![长泽雅美][1]
[1]:https://gitee.com/xsyzer/image_01/raw/master/img/20200416181553.png "长泽雅美"

显示目录：
[TOC]

注脚：
1.使用markdown[^1]
	[^1]:标记语言

表格：
1.可用快捷键Ctrl+T快速插入表格。
2.|第一列|第二列|第三列|


Ctrl+1  一阶标题    Ctrl+B  字体加粗
Ctrl+2  二阶标题    Ctrl+I  字体倾斜
Ctrl+3  三阶标题    Ctrl+U  下划线
Ctrl+4  四阶标题    Ctrl+Home   返回Typora顶部
Ctrl+5  五阶标题    Ctrl+End    返回Typora底部
Ctrl+6  六阶标题    Ctrl+T  创建表格
Ctrl+L  选中某句话   Ctrl+K  创建超链接
Ctrl+D  选中某个单词  Ctrl+F  搜索
Ctrl+E  选中相同格式的文字   Ctrl+H  搜索并替换
Alt+Shift+5 删除线 Ctrl+Shift+I    插入图片
Ctrl+Shift+M    公式块 Ctrl+Shift+Q    引用
Ctrl+Shift+K 代码块


```

## 第一周

问题：如何写空格间距



### 第一节 HTML5基础语法与标签

1. 网页的浏览
   1. ctrl+shift+p ->open with live Server

   2. alt+z自动换行

   3. html骨架结构，DTD：文档类型声明，html标签对，head标签对网页配置，body标签对网页正式内容

   4. 标题和段落标签（换行），div标签（分割）使用

      1. div常见类名

         |   区域   | 类名    |
         | :------: | ------- |
         |   页头   | header  |
         |   logo   | logo    |
         |  导航条  | nav     |
         |   横幅   | banner  |
         | 内容区域 | content |
         |   页脚   | footer  |

         

   5. 网页字符集UTF-8一个汉字占三个字节
      1. gb2312一个汉字占两个字节

   6. 常见的SEO（搜索引擎优化）配置项  title，2个meta标签（discription，keywords）和应该遵守的规则

   7. http是超文本传输协议，浏览器发出http请求，服务器发回http响应，将做好的网页上传到服务器上
2. HTML5特性
   1. 空白折叠现象
   
   2. 转义字符
   
      | 转义字符 | 意义               |
      | :------: | ------------------ |
      |  &lt；   | 小于号             |
      |  &gt；   | 大于号             |
      | &nbsp；  | 空格（不会被折叠） |
      | &copy；  | 版权符号           |
   
   3. HTML注释 ctrl+/

### 第二节 列表标签

1. 无序列表

   1. &lt;ul&gt; 和&lt;li&gt; 必须组合（列表项）

   2. 列表的嵌套

   3. 无序列表的type属性

      1. 已被弃用，建议使用css

         disc 默认实心圆

         circle 空心圆

         square 实心方快

2. 有序列表

   1. &lt;ol &gt;和&lt;li&gt;&gt; 必须组合

   2. 列表的嵌套

   3. &lt;ol &gt;列表的type属性

      1. | type |         意义         |
         | :--: | :------------------: |
         |  a   | 表示小写英文字母编号 |
         |  A   |       大写英文       |
         |  i   |       小写罗马       |
         |  I   |       大写罗马       |
         |  1   |   数字编号（默认）   |

   4. &lt;ol &gt;的start属性

      1. start必须是一个整数，指定了列表编号的起始值，阿拉伯数

   5. &lt;ol &gt;的reversed属性

      1. 列表中的条目是否要倒序排列

3. 定义列表

   1. &lt;dl&gt;和&lt;dt&gt; &lt;dd>
   2. 需要逐条给出定义描述的列表
   3. 使用场景

### 第三节 多媒体与语义化标签

1. 图片与超链接标签

   1. 图片标签&lt;img>标签

      1. src属性，图片路径，图片必须复制到项目文件夹中

      2. alt属性，图片的文本描述，若图片无法加载则会显示alt文本

      3. width,height属性，设置图片宽高，单位像素，可省略

      4. 网页上支持的图片格式

         <center>png是常见的图片格式</center>

         ![image-20210602162828457](C:\Users\Casey\AppData\Roaming\Typora\typora-user-images\image-20210602162828457.png)

      5. 路径回退 ../

   2. 超链接&lt;a>标签

      1. href属性，超文本引用，链接网页网址

      2. title属性，鼠标悬停文本

      3. target属性，设置为blank，在新窗口打开网页

      4. 给图片设置超级链接，&lt;a> 标签包裹 &lt;img>即可

      5. 页面内锚点，较长的页面，可以适当的给h系列标签添加id属性，将其变为页面锚点

         ```html
         <h1 id="monggu">蒙古包</h1>
         ```

         1. 当网址后面添加#时，页面将自动滚动到锚点所在位置

         2. 也可以

            ```html
            <a href = "https://www.baidu.com/#monggu"></a>
            ```

      6. 下载链接，指向exe、zip、rar等文件格式的链接，将自动成为下载链接

         ```html
         <a href="1.zip">下载</a>
         ```

      7. 邮件链接，电话链接

         1. 有mailto：前缀的链接是邮件链接，系统将自动打开email相关软件
         2. 有tel：前缀的链接是电话链接，系统将自动打开拨号盘

2. 音频和视频

   1. 音频和视频&lt;audio>，&lt;video>标签，格式MP3 ogg,mp4 ogv webm

      1. controls属性，播放控件

      2. autoplay属性，自动播放

      3. loop属性，循环播放

         

3. 大纲和语义化标签

   1. 大纲标签
      1. 区块标签
      2. ![image-20210607180650224](C:\Users\Casey\AppData\Roaming\Typora\typora-user-images\image-20210607180650224.png)
      3. header -》divlogo
         1. nav
      4. main
         1. aside
         2. article -》h1,section
      5. footer
   2. 语义化标签
      1. span文本区块标签，行内标签
      2. &lt;b>,&lt;u>,&lt;i>标签
      3. &lt;strong>,&lt;em>,&lt;mark>重要标粗，强调倾斜，高亮标签
      4. &lt;figure>和&lt;figcaption>配套使用

### 第四节 表单标签<form>

1. 表单创建 form  

   1.  <form action="" method="POST"></form>

      ```html
       <form action="" method="POST"></form>
      ```

2. 基本控件

   1. 单行文本框text

      ```html
       <input type = "text" value = "123" disabled>
      <input type = "text" placeholder = "请输入姓名">
      ```

      1.  value属性表示已经填写好的值
      2.  placeholder属性表示提示文本，将以浅色文字写在文本框中，并非文本框的值
      3.  disabled 属性表示用户不能与元素交互，即元素已经锁死
      4.  required 必须填写的
   
   2. 单选按钮radio
   
      ```html
      <input type = "radio"
      ```
   
      1. 单选按钮要有value属性值，向服务器提交的就value值
   
      2. 如果加上checked属性，表示默认被选中 
   
      3. name属性值相同则不同单选按钮会互斥 
   
      4. label标签用来将文字和单选按钮进行绑定，用户单击文字的时候等于点击了单选按钮
   
         ```html
         <label>
         	<input type="radio">女
         </label>
         ```
   
   3. 复选按钮checkbox
   
      1. 复选按钮要有value属性值，向服务器提交
      2. 同组复选按钮name值相同
      3. label进行绑定
   
   4. 下拉菜单select，option
   
      1. select标签表示下拉菜单，option是他的内部选项，option的value值是提交给服务器的
   
   5. 多行文本框textarea
   
      1. textarea表示多行文本框
      2. rows,cols定义多行文本框的行数和列数
   
   6. 三种按钮
   
      1. |                   type属性值                    | 按钮种类 |
         | :---------------------------------------------: | -------- |
         |                     button                      | 普通按钮 |
         | submit （将表单自动提交给在action中定义的页面） | 提交按钮 |
         |                      reset                      | 重置按钮 |
   
   7. 密码框password
   
      1. type属性password
   
3. HTML5新增表单控件

   1. |      type属性值       |       控件       |
      | :-------------------: | :--------------: |
      |         color         |   颜色选择控件   |
      |      date、time       | 日期时间选择控件 |
      |    email（submit）    | 电子邮件输入控件 |
      |         file          |   文件选择控件   |
      |   number（min max）   |   数字输入控件   |
      |   range（min max）    |      拖拽条      |
      |        search         |      搜索框      |
      | url（符合标准的网址） |   网址输入空间   |

   2. datalist 控件

      1. 可以为输入框提供一些备选项，当用户输入的内容与选项的文字相同时，将会显示智能感应。

### 第五节 表格标签 <table>   <tr>  <td>

1. 介绍表格

   1. 表格table，表格行tr，表格数据td

      1. ps：CTRL+shift+d复制当前行

   2. table的border属性 显示边框

      1. ```html
         <table border=4>  
         <style>
                 table,tr,td{
                     border-collapse: collapse;
                 }
             </style
         ```

   3. table的caption属性

      1. caption表格标题，通常作为第一个子元素

   4. th每一列标题表格 和td同一级别

2. 单元格的合并

   1. colspan属性，用来设置td或者th的列跨度
   2. rowspan属性，用来设置td或者th的行跨度

3. 表格其他特性

   1. thead定义表头
   2. tbody定义表的核心内容
   3. tfoot定义表脚，汇总行
   4. cellspacing cellpadding

## 小医生项目开发

1. 工作开发流程
   1. 产品经理：提出需求，画出原型
   2. 设计师：画设计图Axure或者Sketch
   3. 前端开发
   
   

