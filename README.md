## 概述

### 定义

   Hyper Text Markup language超文本标记语言，用于描述页面结构的语言

   Cascading Style Sheets层叠式样式表，用于描述页面长什么样子

### 学习态度

1. 心态平和
2. 多练习
3. **不要你以为懂了，就可以不练习，这是IT领域常常出现的幻觉**

### 一些术语

1. web  --->  互联网
2. **w3c  ---> 万维网联盟，非盈利性的组织，为互联网提供各种标准**
3. XML  ---> 可扩展的标记语言，Extension Markup Language，用来定义文档结构，相对于HTML而言，他可以自定义标签
4. **MDN  ---> 可以查一些资料，官方定义和解释**

### 浏览器

1. shell：外壳
2. **core：内核  ---> (渲染引擎，js引擎，其他模块)**

### 主流浏览器

| 主流浏览器    | 内核                                                         |
| ------------- | :----------------------------------------------------------- |
| IE            | trident                                                      |
| Firefox       | Gecko                                                        |
| Google chrome | Webkit(谷歌和苹果联合开发的)/blink(与苹果公司分歧后，自己研发的) |
| Safari        | Webkit                                                       |
| Opera         | presto(以前)/blink(现在)                                     |

## HTML核心1

### 基础知识

元素（也就是常说的标签） = 起始标记 + 结束标记 + 元素内容 + 元素属性

属性 = 属性名 + 属性值

属性的分类：

1. 局部属性：某些元素特有
2. 全局属性：每个元素都有

有些元素没有结束标记，这样的元素叫做：**空元素**

空元素的写法有两种：

1. ~~~html
   <img src="">html5
   ~~~

2. ~~~html
   <img src="" />以前的写法
   ~~~

元素的关系：

1. 父元素（爸爸）
2. 子元素（儿子）
3. 祖先元素（爹）
4. 子孙元素（孙子）
5. 兄弟元素（哥哥姐姐弟弟妹妹）

~~~html
<!DOCTYPE html>
    文档声明，告诉浏览器，当前浏览器使用的HTML的标准是5；不写的话，将导致浏览器进入怪异渲染模式，可能显示不正常
<html lang="en">
    根元素，一个页面只有一个，并且该元素是所有元素的父元素或祖先元素，HTML5中没有强制写这个元素
    lang="en"表示language，全局属性，表示该元素内部的文字是使用哪一种自然语言书写的
    lang="cmn-hans"表示中国官方语言，简体（simple）汉语（han）/也可以这么写lang=“zh-CN”但是已经过时了
<head>文档头部，不会显示在页面上
    meta元素表示文档的元数据：附加属性
    <meta charset="UTF-8">charset
    是局部属性，告诉网页用的是哪一个字符编码表，也就是UTF-8,相当于一个字典
    比如说中国使用的是GB2312，台湾是GBK
    UTF-8是Unicode的一个版本，也就是万国码，包含所有的语言
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    适配手机端的
    <title>Document</title>
    表示的是网页标题
</head>
<body>
    文档体
</body>
</html>
~~~

### 语义化

每个元素都有本身的含义

1. a元素：链接（当然还有别的作用，但是用的最多的是链接）
2. p元素：段落
3. h1：一级标题

元素与展示效果无关

   元素展示到页面上应该由css来控制

   因为浏览器带有默认的css样式，所以每个元素都有一些默认的样式

   比如你写h1的时候，里面的内容就会显示很大，并且加粗，这些都是css控制的，可以改的

   **重要：选择什么元素，取决于内容的含义，而不是展示的效果**## 概述

### 定义

   Hyper Text Markup language超文本标记语言，用于描述页面结构的语言

   Cascading Style Sheets层叠式样式表，用于描述页面长什么样子

### 学习态度

1. 心态平和
2. 多练习
3. **不要你以为懂了，就可以不练习，这是IT领域常常出现的幻觉**

### 一些术语

1. web  --->  互联网
2. **w3c  ---> 万维网联盟，非盈利性的组织，为互联网提供各种标准**
3. XML  ---> 可扩展的标记语言，Extension Markup Language，用来定义文档结构，相对于HTML而言，他可以自定义标签
4. **MDN  ---> 可以查一些资料，官方定义和解释**

### 浏览器

1. shell：外壳
2. **core：内核  ---> (渲染引擎，js引擎，其他模块)**

### 主流浏览器

| 主流浏览器    | 内核                                                         |
| ------------- | :----------------------------------------------------------- |
| IE            | trident                                                      |
| Firefox       | Gecko                                                        |
| Google chrome | Webkit(谷歌和苹果联合开发的)/blink(与苹果公司分歧后，自己研发的) |
| Safari        | Webkit                                                       |
| Opera         | presto(以前)/blink(现在)                                     |

## HTML核心1

### 基础知识

元素（也就是常说的标签） = 起始标记 + 结束标记 + 元素内容 + 元素属性

属性 = 属性名 + 属性值

属性的分类：

1. 局部属性：某些元素特有
2. 全局属性：每个元素都有

有些元素没有结束标记，这样的元素叫做：**空元素**

空元素的写法有两种：

1. ~~~html
   <img src="">html5
   ~~~

2. ~~~html
   <img src="" />以前的写法
   ~~~

元素的关系：

1. 父元素（爸爸）
2. 子元素（儿子）
3. 祖先元素（爹）
4. 子孙元素（孙子）
5. 兄弟元素（哥哥姐姐弟弟妹妹）

~~~html
<!DOCTYPE html>
    文档声明，告诉浏览器，当前浏览器使用的HTML的标准是5；不写的话，将导致浏览器进入怪异渲染模式，可能显示不正常
<html lang="en">
    根元素，一个页面只有一个，并且该元素是所有元素的父元素或祖先元素，HTML5中没有强制写这个元素
    lang="en"表示language，全局属性，表示该元素内部的文字是使用哪一种自然语言书写的
    lang="cmn-hans"表示中国官方语言，简体（simple）汉语（han）/也可以这么写lang=“zh-CN”但是已经过时了
<head>文档头部，不会显示在页面上
    meta元素表示文档的元数据：附加属性
    <meta charset="UTF-8">charset
    是局部属性，告诉网页用的是哪一个字符编码表，也就是UTF-8,相当于一个字典
    比如说中国使用的是GB2312，台湾是GBK
    UTF-8是Unicode的一个版本，也就是万国码，包含所有的语言
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    适配手机端的
    <title>Document</title>
    表示的是网页标题
</head>
<body>
    文档体
</body>
</html>
~~~

### 语义化

每个元素都有本身的含义

1. a元素：链接（当然还有别的作用，但是用的最多的是链接）
2. p元素：段落
3. h1：一级标题

元素与展示效果无关

   元素展示到页面上应该由css来控制

   因为浏览器带有默认的css样式，所以每个元素都有一些默认的样式

   比如你写h1的时候，里面的内容就会显示很大，并且加粗，这些都是css控制的，可以改的

   **重要：选择什么元素，取决于内容的含义，而不是展示的效果**
