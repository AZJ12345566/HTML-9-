# HTML-9-
HTML JavaScript、路径、头部
//HTML JavaScript
  //HTML JavaScript使HTML页面更具动态性和交互性
  //实例
  <html>
  <body>

  <h1>我的第一段JavaScript<h1>

  <button type="button"
  onclick="document.getElementById('demo').innerHTML=Date()">
  点击我来显示日期和时间
  </button>

  <p id="demo"></p>
  </body>
  </html>

  //HTML<script>标签
  //HTML<script>标签用于定义客户端脚本
  //<script>元素即可包含脚本语句，也可以通过src属性指向外部脚本文件
  //JavaScript的创建用途是图像处理，表单验证和内容的动态更改
  //如需选取HTML元素，JavaScript最常用document.getElementById()方法
  //这个JavaScript示例向"id=demo"的元素内写入"Hello JavaScript";
  <html>
  <body>

  <h1>使用JavaScript更改文本</h1>

  <p>本例把"Hello JavaScript!"写入id="demo"的HTML元素内</p>

  <p id="demo"</p>

  <script>
  document.getElementById("demo").innerHTML="Hello JavaScript!";
  </script>
  </body>
  </html>

  //JavaScript的味道
  //实例：JavaScript能够更改内容
  <html>
  <body>

  <h1>我的第一段 JavaScript</h1>

  <p>JavaScript可以更改HTML的内容：</p>
  <botton type="button"onclick="myFunction()">点击我！</botton>

  <p id="demo">这是一个演示。</p>

  <script>
  function myFunction(){document,getElementById("demo").innerHTML="Hello JavaScript!";}
  </script>
  </body>

  //实例：JavaScript能够更改样式
  <html>
  <body>

  <h1>我的第一段JavaScript</h1>

  <p id="demo">JavaScript 可以更改HTML元素的样式。</p>

  <script>
  function myFunction(){
    document.getElementById("demo").style.fontSize="25px";
    document.getElementById("demo").style.color="red";
    document.getElementById("demo").style.backgroundColor="yellow";
  }
  </script>

  <button type="button"onclick="myFunction()">点击我！</button>
  </body>
  </html>

  //JavaScript能够更改属性
  <html>
  <body>

  <h1>我的第一段JavaScript</h1>
  <p><在这里，JavaScript更改了图像的src属性。</p>

  <script>
  function light(sw){
    var pic;
    if(sw==0){
      pic="i/eg_bulboff.gif"
    }
    else{
      pic="/i/eg_bulbon.gif"
    }
    document.getElementById('myImage').src=pic;
  }
  </script>

  <img id="myImage" src="/i/eg_bulboff.gif"width="109" hright="180">
  <p>
    <button type="button"onclick="light(1)">开灯</button>button>
    <button type="button"onclick="light(0)">关灯</button>button>
  </p>
  </body>
  </html>

  //标签积累
  //<script>定义客户端脚本
  //<noscript>为不支持客户端脚本的用户定义替代内容

//HTML文件路径
  //路径                            描述
  //<img src="picture.jpg">            picture.jpg位于当前网页相同的文件夹
  //<img src="images/picture.jpg">     picture.jpg位于当前文件夹的images文件夹中
  //<img src="/images/picture.jpg">    picture.jpg位于当前站点根目录的images文件夹中
  //<img src="../picture.jpg">         picture.jpg位于当前文件夹的上一级文件夹中

  //HTML文件路径
    //文件路径描述了网站文件夹结构中某个文件的位置
    //文件路径会在链接外部文件时被用到
    //1.网页 2.图像 3.样式表 4.JavaScript

  //绝对文件路径
  //绝对文件路径是指向一个因特网文件的完整URL：
  //实例：
  //<img src="https://www.w3school.com.cn/images/picture.jpg"alt="flower">
  //<img>标签以及src和alt属性在HTML图像这一章做了详解

  //相对路径
  //相对路径指向了位于当前网站根目录中images文件夹里的一个文件：
  //实例：
  <img src="images/picture.jpg"alt="flower">
  //在本例中，文件路径指向了位于当前文件夹的上一级文件夹中images文件夹里的一个文件：
  <img src="../images/picture.jpg"alt="flower">

  //使用相对路径是一个好习惯
  //如果使用了相对路径，那么你的网页就不会与当前的基准URL进行绑定。所有链接在你的电脑上或未来的公共域中均可正常工作

//HTML头部元素
  //亲自试一试-实例(5个待输入)

  //HTML<head>元素
  //<head>元素是所有头部元素的容器。<head>内的元素可包含脚本，指示浏览器在何处可以找到样式表，提供元信息，等等。
  //以下标签都可以添加到head部分：<title>,<base>,<link>,<meta>,<script>,<style>

  //HTML<title>元素
  //<title>标签定义文档标题
  //title元素在所有HTML/XHTML文档中都是必需的

  //title元素能够：
  //1.定义浏览器工具栏中的标题
  //2.提供页面被添加到收藏夹时显示标题
  //3.显示在搜索引擎结果中的页面标题

  //HTML<base>元素
  //<base>标签为页面上的所有链接规定默认地址或默认地址(target):
  <head>
  <base href="http://www.w3schoo;.com.cn/images/"/>
  <base target="_blank"/>
  </head>

  //HTML<link>元素
  //<link>标签定义文档与外部资源之间的关系
  //<link>标签最常用于链接样式表：
  <head>
  <link rel="stylesheet"type="text/css"href="mystyle.css"/>
  </head>

  //HTML<style>元素
  //<style>标签用于为HTML文档定义样式信息
  //你可以在style元素内规定HTML元素在浏览器中呈现的样式：
  <head>
  <style type="text/css">
  body{background-color:yellow}
  p{color:blue}
  </style>
  </head>

  //HTML<meta>元素
  //元数据(metadata)是关于数据的信息。
  //<meta>标签提供关于HTML文档的元数据。元数据不会显示在页面上，但对手机可读
  //典型的情况是，meta元素被用于规定页面的描述、关键词、文档的作者、最后修改时间以及其他与元数据
  //<meta>标签始终位于head元素中
  //元数据可用于浏览器(如何显示内容或重新加载页面)，搜索引擎(关键词)，或者web服务

  //HTML<script>元素
  //<script>标签用于定义客户端脚本，比如JavaScript

  //HTML头部元素
  //<head>:定义关于文档的信息
  //<title>：定义文档标题
  //<base>：定义页面上所有链接的默认地址或默认目标
  //<link>：定义文档与外部资源之间的关系
  //<meta>：定义关于HTML文档的元数据
  //<script>：定义客户端脚本
  //<style>：定义文档的样式信息
