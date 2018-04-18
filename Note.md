# 1. 认识HTML

- html 结构，CSS 样式
- #d2b48c 十六进制码
- CSS 中的“body"表示｛｝中的所有 CSS 要应用于 HTML  body 元素中的内容，即主体中的内容。


- Q: border: 2px red; 
 为什么显示不出来？

- CSS： 好的设计和布局有利于页面的可读性和可用性
- 记得幼儿园课里有讲过html和css是结构和样式分离
- HTML 和 CSS 是我们用来创建网页的语言。
- Web服务器存储并提供由HTML和CSS创建的网页。浏览器获取页面，并根据HTML和CSS显示网页的内容。P36
- HTML是超文本标记语言（HyperText Markup Language）的缩写，用来建立网页的结构。
- CSS是层叠样式表（Cascading Style Sheets)的缩写，用来控制HTML的表现。
- 元素: 标记名+尖括号+内容; " h1 /h1 "成对的匹配标记：告诉浏览器页面的结构;
  有些元素除外，如 img 。
- 开始标记可以有属性。
- 所有页面都要有一个 html 元素，其中要有一个 head 元素和一个  body 元素。
- 网页的信息放在 head 元素里。
- body 元素里的内容就是你将在浏览器里看到的东西。
- 大多数空白符 （制表符、回车、空格）都会被浏览器忽略，不过可以利用空白符让你的HTML更有可读性。
- style 元素总要放在 head 元素里。
- 可以使用CSS在HTML中指定元素的特性。
- em 元素： emphasize 强调：显示斜体; P92: 显示斜体，不好用，可以用别的方式。

## 填字游戏: P37
记英语单词，方便以后看英文。    

1. Q: heading: 一共有6个
3. presentation 表现：要控制表现时，会使用CSS。应该就是样式。
4. 结构 Struture
6. Q: 50SKITSCH
8. attribute 属性
10. whitespace 空白符
12. 通过STYLE来控制表现。
15. element
16. tag标记

# 2 深入了解超文本
HT(Hyper Text) : 链接到其他页面（文本）的文本

## 2.1 创建链接
<a>元素和href属性

####  a 元素
【想像成 at 】
 - 作用：创建链接。  a  /a 中的内容：链接文本，或者说标签，显示有下划线，【也就是网页上显示可单击的文本或图片，带链接的文字或图片】。
 

#### href 属性
 - 本义：词典：“abbr. 超文本引用（hypertext reference）；超链接” ;
 - 作用：通过href=""指定链接的目标文件;  
 - 格式： a href="要链接的文件">文本 /a ;
 - 目标文件：可以是html，图片，也可以是pdf等各种资源。
 - 运行：单击一个链接时，浏览器会加载href属性中指定的Web页面。
  

## 属性：
关于属性的理解

### 组成
- 属性名：如href;
- 等于号=;
- 属性值：用""括起来

### 原理
【这相当于JS里的对象的逻辑。也是，任何事物都是带着属性的。如果要表示事物，则会表示其属性;区别在于，表示的形式不同而已。】

### 相关
- HTML5支持定制数据属性，包括属性名。【Q:意思是说，HTML5可以自己定制属性？】
- 元素有自己的属性
- 属性就是功能:元素是结构，属性是元素的功能，也就是具体结构的功能。

### 其他
- img src ="" 可以单独用，比如 [这里](lounge.html) ;  
  也可以放在a元素里，P55。例子以后找，Q。

## 2.2 用文件夹组织网站

- 组织文件的依据：灵活，可扩展，简单
- 在网站构建初期组织文件

### 链接路径
- 相对路径：从包含这个链接的页面开始，沿着一条路径，经过一些文件夹直到找到你需要指向的那个文件。
- “../” ： 上级文件夹、上行一个文件夹。第一个点指本文件夹，第二个点指上一层文件夹。  
  上行一个文件夹找另一个文件夹，或者说“上一级目录里的另一个文件夹”
  “../..” ：上行两级文件夹
- Web中的斜杠只有“/”，通用分隔符
- 有关路径的长度，对于大型网站，规范中建议当心超过255个字符。【Q:什么规范 ？】
- 不要使用空格

### 题外：关于 Git
![新建文件夹时，commit后的显示](Note-Images/git-when-creat-folder-of-images.jpg)

# 3.构建模块

- 基本构建模块：h1、h2、h3、p等
- 从大的结构元素来考虑页面的构成：标题、段落、图像，等等。

## 构建Web步骤:  
第一、二章也是这样，只是这一章重点讲。

1. 草图：【内容的布局：需要表现的内容，列一下大概的表现形式。标题、图片、段落，这些要怎么放。其实就是排版】
2. 略图：【html结构略图：抽象成html模块要怎么排版】
3. 网页：【html文档：用html元素确定的网页】


### 学习新元素
#### q 引用元素

- 格式：自动在浏览器页面加“”;但有的浏览器不会自动加“”;非英语语言有相应的显示，不一定是“”。
- 作用：
  - 短引用，在 p 段落里;
  - 设置引用的样式;
  - 用最合适的方式来显示引用内容【添加有关引用的拓展功能】，比如，移动设备的显示，语音HTML功能和大屏幕阅读器【Q:找例子】，或搜索引擎可搜寻包含引用的网页。

#### blockquote 引用元素
- 格式：换行，具体样式自定义，目前在Chrome里是“空一行，过一行，空一行”，跟教材上一样，如下图：
![](./images/breakEl-looking.jpg)
- 作用：
  - 单独长引用; 在段落外，自成一段
  - 内部可多段，用 p 元素;
  - 内部可用 q ，例如，引用块中引用了别人的话。嵌套引用。
  - 指定样式，因为不同浏览器对 blockquote 的显示不一样。
     - 有些浏览器会缩进;

## 页面文本流
【页面布局 和 元素 的关系，元素在文本中】
### 元素 分类方式1：
  - 内联（inline）元素 : 
    - 作用：标记小段内容;
    - 形式：在行内出现;【行内表现】 ,跟其包含元素的其余内容放在一起。
    - 如： img、q 、 a 、 em 等
  - 块（block）元素：
    - 作用：Web页面中的主要构建模块;
    - 形式：前后各有一个换行;
    - 如： blockquote 、 h1、a、ul、li、ol、... p 等
    - 【HTML的换行用块元素的使用来u现，让网页在浏览器上的显示宽度可自由调整】：  
       在HTML文件中的换行符不会出现，使用块元素，浏览器就会使用换行符来分隔每一“块”
  - br：模糊地带
### 元素在布局上的选用: 
  - 设计一个页面时，一般先从较大的块开始（块元素），然后在完善页面时再加入内联元素。
  - 在用CSS控制HTML表现时，区分好内联元素和块元素，可以轻松设计好布局。


####  br 元素
换行
【联想： line break：换行符 】
- 形式：只有开始标记，没有内容的元素。简写
- 作用：只是换行
- 与 br/ 作用一样。 br/ 与XHTML兼容，语法更严格。HTML中使用 br 。【对教材中内容提取还不够严谨，等了解XHTML再说】

### 元素 分类方式2：
  - 正常元素
  - void 元素
    - 空元素，无内容，无值
    -  img  、 br 

## 心法
选择与内容结构含义最接近的HTML元素。产生更大的能力和灵活性。


#### HTML列表
-  li ： li 每个列表项 /li   (list item)
  - 列表项在 p 段落外
    ![](./Note-Images/li-el-only.png)
- 包围所有列表项:归为一组
  -  ol 元素：有序列表(order list)
   - 自动编号
  -  ul 元素：无序列表(unordered list)
    - 最好不要用不同的项目符号。待CSS部分讲。
  ![](./Note-Images/oi-and-ul-el-tags.jpg)
  ![](./Note-Images/oi-and-ul-el.jpg)
  - 都只能包含 li 

-- 都属于块元素
-- 最好把 /p 放在下一行
![](./Note-Images/p-break.jpg)
-- 可以嵌套
![](./Note-Images/list-nested.jpg)

- 定义列表
 -  dl :定义术语
 -  dt :定义描述
```
Bruna Shave Signs
     Road Signs common in the U.S. in the 1920s and 1930s advertising shaving products.
Route 66
     Most famous road in the U.S. highway system.
```

## 心法 - 嵌套关系
### 关系：
- html 
  - head 
    - title
  - body
    - p 
      - q
      - em

### 相关：
- 确保标记匹配
- 提到 工业强度的HTML

#### 字符实体 【Q】
character entity
- 是一种简写缩写
- 分为 实体名 和 编号缩写
- 浏览器显示的字符，如果是html、md中的标记，那么，在html、md等文件里需要用实体字符代替。

查询地址1：
<a href="http://www.w3schools.com/tags/ref_entities.asp">http://www.w3schools.com/tags/ref_entities.asp</a>

查询地址2：
<a href="http://www.unicode.org/charts">http://www.unicode.org/charts</a>

自动翻译地址：
<a href="http://www.w3schools.com/tags/ref_entities.asp">http://www.w3schools.com/tags/ref_entities.asp</a>

需要运行环境支持相应的字体

#### 复习
- 空元素没有内容。不过它有开始和结束。
=> 不就是 br 和 img这类有开始没有结束的吗？还是说，只没有放内容？

# 4. Travel the Web
### 域名： 
starbuzz.com 是域名， www.starbuzz.com, corporate.starbuzz.com是网站。
同一个域名上的不同前缀是不同网站。
### 根文件夹
- 根文件夹是页面的顶级文件夹。  
- 在Web服务器上，根文件夹中的内容可以从网上访问到。
- 根文件夹可能有不同的名字，但最重要是，知道在哪里。
- 把根文件夹全部复制到对应网站的根文件夹下。
  - 通过FTP文件传输方法 (file transfer protocol)

### 用FTP传输
- cd 切换到目标文件夹
- put 将文件传到服务器
- mkdir 创建新目录
- get 获取文件
- dir 得到当前目录的文件列表，查看文件夹
- pwd 查看当前路径
- bye 退出


  

  

    
