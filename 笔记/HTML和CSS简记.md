# 1.HTML介绍

## 1.C/S架构与B/S架构

1. C/S架构，特点：需要安装，偶尔更新，不跨平台、开发更具有针对性。
2. B/S架构，特点：无需安装，无需更新，可跨平台，开发更具有通用性。

>  名词解释：C => client（客户端）、B => browser（浏览器）、S => server（服务器）。
>
> 服务器 ：为软件提供数据的设备（在背后默默的付出）。



## 2.HTML发展史

![image-20230427083503115](/Users/kaiqiang/Library/Application Support/typora-user-images/image-20230427083503115.png)



## 3.HTML设置语言

1. 作用：

   1. 让浏览器显示对应的翻译提示。
   2. 有利于搜索引擎优化。

2. 具体代码：

   ```html
   <html lang="zh-CN">
   ```

3. VScode默认设置——生成html代码是默认生成```<html lang='zh-CN'>```

   <img src="/Users/kaiqiang/Library/Application Support/typora-user-images/image-20230426200047977.png" alt="image-20230426200047977" style="zoom:25%;" />

4. 扩展知识

   > 1. 第一种写法（ 
   >
   > 语言-国家/地区 ），例如：
   >
   > zh-CN ：中文-中国大陆（简体中文）
   >
   > zh-TW ：中文-中国台湾（繁体中文）
   >
   > zh ：中文
   >
   > en-US ：英语-美国
   >
   > en-GB ：英语-英国
   >
   > 2. 第二种写法（ 
   >
   > 语言—具体种类）已不推荐使用，例如：
   >
   > zh-Hans ：中文—简体
   >
   > zh-Hant ：中文—繁体
   >
   > 3. W3School 上的说明：**《语言代码参考手册》**、**《国家****/****地区代码参考手册》**
   >
   > 4. W3C官网上的说明：**《****Language tags in HTML****》** 



## 4.HTML标准结构

1. 标准结构：

   ```html
   <!DOCTYPE html>
   <html lang="zh-CN">
     <head>
       <meta charset="UTF-8"> 
       <title>我是一个标题</title>
     </head> 
     <body> 
     </body> 
   </html>
   ```

2. 编码与解码模式——UTF-8

   1. UTF—8:是'万国码'，使用最广泛
   2. 数据出现？？？是编码出现问题，数据是就已经丢失，出现乱码是编码出现问题，数据还可解码





# 2.HTML基础

## 1.排版标签

​	<img src="/Users/kaiqiang/Library/Application Support/typora-user-images/image-20230427085745574.png" alt="image-20230427085745574" style="zoom:50%;" />

1. h1 最好写一个， h2~h6 能适当多写。
2. h1~h6 不能互相嵌套，例如： h1 标签中最好不要写 h2 标签了。
3. p 标签很特殊！它里面不能有： h1~h6 、 p 、 div 标签



## <span style='color:red'> 2.语义化标签</span>

1. 概念：合适的地方使用合适的标签，img中alt属性也是图片标签
2. 原则：标签的默认样式不重要(css都可以修改)
3. 优势：
   1. 代码结构清晰可读性强。
   2. 有利于 **SEO**（搜索引擎优化）。
   3. 方便设备解析（如屏幕阅读器、盲人阅读器等）。



## 3.块状元素和行内元素

1. 块状元素：独占一行(内部可以写：块状元素、行内元素)
2. 行内元素：不独占一行(内部可以写行内元素，不可以写块状元素)



## 4.常用标签

1. 常用标签样式不重要，主要是他的标签语义

![image-20230427091927552](/Users/kaiqiang/Library/Application Support/typora-user-images/image-20230427091927552.png)



## 5.文本标签——不常用

<img src="/Users/kaiqiang/Library/Application Support/typora-user-images/image-20230427092133384.png" alt="image-20230427092133384" style="zoom:50%;" />

> 1. 这些不常用的文本标签，编码时不用过于纠结（酌情而定，不用也没毛病）。
> 2. blockquote 与 address 是块级元素，其他的文本标签，都是行内元素。
> 3. 有些语义感不强的标签，我们很少使用，例如：small 、 b 、 u 、 q 、 blockquote
> 4. HTML标签太多了！记住那些：重要的、语义感强的标签即可；截止目前，有这些：h1~h6 、 p 、 div 、 em 、 strong 、 span 



## 6.图片标签

1. 基本使用

   <img src="/Users/kaiqiang/Library/Application Support/typora-user-images/image-20230427092512199.png" alt="image-20230427092512199" style="zoom:50%;" />

   > 1. 尽量不要修改图片的宽高，会导致图片比例失调
   > 2. 使用alt属性
   >    1. 搜索引擎通过 alt 属性，得知图片的内容。—— 最主要的作用。
   >    2. 当图片无法展示时候，有些浏览器会呈现 alt 属性的值。
   >    3. 盲人阅读器会朗读 alt 属性的值。

2. 常见图片格式

   1. .jpg:目前最常用

   2. .png:使用透明背景，使用png图片

   3. .bmp:主要在游戏中使用

   4. .gif:使用动图

   5. .webp：未来的其实(解决浏览器不支持webp方法：准备两张图片)

   6. .base64

      > 图片详情在 尚硅谷—笔记中查看



## 7.超链接

主要作用：当前页面跳转

可以实现：：①跳转到指定页面、②跳转到指定文件（也可触发下载）、③跳转到锚点位置、④唤起指定应用。

<img src="/Users/kaiqiang/Library/Application Support/typora-user-images/image-20230427093931460.png" alt="image-20230427093931460" style="zoom:50%;" />

1. 页面跳转

   ```html
   <!-- 跳转其他网页 -->
   <a href="https://www.jd.com/" target="_blank">去京东</a>
   
   <!-- 跳转本地网页 -->
   <a href="./10_HTML排版标签.html" target="_self">去看排版标签</a>
   ```

   > 1. 代码中的**多个空格**、**多个回车**，都会被浏览器解析成一个空格！
   >
   > 2. 虽然 a 是行内元素，但 a 元素可以包裹除它自身外的任何元素！

2. 跳到指定文件

   ```html
   <!-- 浏览器能直接打开的文件 -->
   <a href="./resource/自拍.jpg">看自拍</a>
   <a href="./resource/小电影.mp4">看小电影</a>
   <a href="./resource/小姐姐.gif">看小姐姐</a> 
   <a href="./resource/如何一夜暴富.pdf">点我一夜暴富</a>
   
   <!-- 浏览器不能打开的文件，会自动触发下载 -->
   <a href="./resource/内部资源.zip">内部资源</a>
   
   <!-- 强制触发下载 -->
   <a href="./resource/小电影.mp4" download="电影片段.mp4">下载电影</a>
   ```

   > 注意点1:浏览器无法打开的资源，就直接下载
   >
   > 注意点2:download可以强制下载

3. 锚点

   具体使用：

   1. 设置锚点```<a name='texst'>```(推荐使用id定位，因为更加精准)

   2. 跳转```<a href="#text">```

      > 锚点详情在 尚硅谷—笔记中查看

4. 唤起设备

   a标签可以唤起应用程序

   ```html
   <!-- 唤起设备拨号 -->
   <a href="tel:10010">电话联系</a>
   <!-- 唤起设备发送邮件 -->
   <a href="mailto:10010@qq.com">邮件联系</a> 
   <!-- 唤起设备发送短信 -->
   <a href="sms:10086">短信联系</a>
   ```

   







