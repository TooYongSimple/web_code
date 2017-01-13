# Html介绍

### 1.Html和CSS关系
1. HTML是网页内容的载体。内容就是网页制作者放在页面上想要让用户浏览的信息，可以包含文字、图片、视频等。

2. CSS样式是表现。就像网页的外衣。比如，标题字体、颜色变化，或为标题加入背景图片、边框等。所有这些用来改变内容外观的东西称之为表现。

3. JavaScript是用来实现网页上的特效效果。如：鼠标滑过弹出下拉菜单。或鼠标滑过表格的背景颜色改变。还有焦点新闻（新闻图片）的轮换。可以这么理解，有动画的，有交互的一般都是用JavaScript来实现的。

### 2.认识html文件基本结构
1. \<html>\</html>称为根标签，所有的网页标签都在\<html>\</html>中。

2. \<head> 标签用于定义文档的头部，它是所有头部元素的容器。头部元素有\<title>、\<script>、 \<style>、\<link>、 \<meta>等标签。

3. 在\<body>和\</body>标签之间的内容是网页的主要内容，如\<h1>、\<p>、\<a>、\<img>等网页内容标签，在这里的标签中的内容会在浏览器中显示出来。

### 3.认识head标签
~~~
<head>
    <title>...</title>
    <meta>
    <link>
    <style>...</style>
    <script>...</script>
</head>
~~~

**\<title>**标签：在\<title>和\</title>标签之间的文字内容是网页的标题信息，它会出现在浏览器的标题栏中。网页的title标签用于告诉用户和搜索引擎这个网页的主要内容是什么，搜索引擎可以通过网页标题，迅速的判断出网页的主题。每个网页的内容都是不同的，每个网页都应该有一个独一无二的title。

### 4.了解html代码注释
	<!--注释文字 -->
	
### 5.各种标签————第一部分
1. \<body>标签：在网页上要展示出来的页面内容一定要放在body标签中
2. \<p>标签：如果想在网页上显示文章，这时就需要\<p>标签了<p>这是一段p标签里的内容</p>
3. \<hx>标签:标题标签一共有6个，h1、h2、h3、h4、h5、h6分别为一级标题、二级标题、三级标题、四级标题、五级标题、六级标题。并且依据重要性递减。\<h1>是最高的等级.<h1>这是一级标题</h1><h6>这是6级标题</h6>
4. \<em> 和 \<strong> 但两者在强调的语气上有区别:\<em> 表示强调，\<strong> 表示更强烈的强调。并且在浏览器中\<em> 默认用斜体表示，\<strong> 用粗体表示<br><em>这是斜体</em> <br / > <strong>这是粗体</strong>
5. \<span>标签:\<span>标签是没有语义的，它的作用就是为了设置单独的样式用的。
6. \<q>标签:短文本引用,注意要引用的文本不用加双引号;<br /> <q>这是一段引用的话</q>
7. \<blockquote>标签:长文本引用 <br /> <blockquote>暗淡轻黄体性柔，<br >情疏迹远只香留。<br />何须浅碧深红色，<br />自是花中第一流。</blockquote>
8. 使用\<br>标签分行显示文本:与以前我们学过的标签不一样，\<br />标签是一个空标签，<br />没有HTML内容的标签就是空标签，空标签只需要写一个开始标签，这样的标签有\<br />、\<hr />和\<img />。
9. \&nbsp: 可以为网页添加空格;
10. \<hr />标签的在浏览器中的默认样式线条比较粗，颜色为灰色，可能有些人觉得这种样式不美观，没有关系，这些外在样式在我们以后学习了css样式表之后，都可以对其修改。<hr />
11. \<address>联系地址信息\</address> <address>北京市朝阳区广渠门外大街
12. 使用\<code>标签来插入一行代码：\<code>var i=i+300;\</code>  <code> var i = i+300;</code>
13. 使用\<pre>标签来插入大段代码：<pre>
var message="欢迎";
for(var i=1;i<=10;i++)<br>
{<br>
         alert(message); <br>
}<br>
</pre>


### 6.各种标签————第二部分

1. ul-li标签：这些列表就可以使用ul-li标签来完成。ul-li是没有前后顺序的信息列表。 <pre>
\<ul>
  \<li>信息\</li>
  \<li>信息\</li>
   ......
\</ul>
</pre> <ul> <li>123456789<li>987654321</ul>

2. \<ol>标签：有序列表：<ol> <li>123456789</li> <li>987654321</li> </ol>
3. \<div>标签：在网页制作过程过中，可以把一些独立的逻辑部分划分出来，放在一个\<div>标签中，这个\<div>标签的作用就相当于一个容器。
4. \<div>标签的命名：在上一小节中，我们把一些标签放进\<div>里，划分出一个独立的逻辑部分。为了使逻辑更加清晰，我们可以为这一个独立的逻辑部分设置一个名称，用id属性来为\<div>提供唯一的名称，这个就像我们每个人都有一个身份证号，这个身份证号是唯一标识我们的身份的，也是必须唯一的。<code>\<div  id="版块名称">…………\</div></code> <br /> **举个栗子🌰** <pre>\<div id="hotlist">
   \<h2>热门课程排行榜\</h2>
    \<ol>
       \<li>前端开发面试心法 \</li>
       \<li>零基础学习html\</li>
       \<li>javascript全攻略\</li>
    \</ol>
\</div>
\<div id="learninginstructed">
    \<h2>web前端开发导学课程\</h2>
    \<ul>
       \<li>网页专业名词大扫盲 \</li>
       \<li>网站职位定位指南\</li>
       \<li>为您解密Yahoo网站制作流程\</li>
    \</ul>
\</div>
</pre>

5. \<table>标签：创建表格的四个元素：table、tbody、tr、th、td <pre>
	1、\<table>…\</table>：整个表格以\<table>标记开始、\</table>标记结束。<br>
	2、\<tbody>…\</tbody>：当表格内容非常多时，表格会下载一点显示一点，但如果加上\<tbody>标签后，这个表格就要等表格内容全部下载完才会显示。如右侧代码编辑器中的代码。<br>
	3、\<tr>…\</tr>：表格的一行，所以有几对tr 表格就有几行。<br>
	4、\<td>…\</td>：表格的一个单元格，一行中包含几对\<td>...\</td>，说明一行中就有几列。<br>
	5、\<th>…\</th>：表格的头部的一个单元格，表格表头。<br>
	6、表格中列的个数，取决于一行中数据单元格的个数.<br>
	总结:<br>
	1、table表格在没有添加css样式之前，在浏览器中显示是没有表格线的<br>
	2、表头，也就是th标签中的文本默认为粗体并且居中显示。</pre>
	**举个栗子🌰**
	<style type="text/css">
	  table tr td,th{border:1px solid #111;}
	</style>
	
	<table>
	  <tbody>
	  <tr>
	  	<th>产品名称</th>
	  	<th>品牌</th>
	  	<th>库存量（人）</th>
	  	<th>入库时间</th>
	  </tr>
	  <tr>
	  	<td>耳机</td>
	  	<td>联想</td>
	  	<td>12</td>
	  	<td>2016</td>
	  </tr>
	  <tr>
	  	<td>U盘</td>
	  	<td>金士顿</td>
	  	<td>20</td>
	  	<td>2017</td>
	  </tr>
	  <tr>
	  	<td>U盘</td>
	  	<td>金士顿</td>
	  	<td>30</td>
	  	<td>2018</td>
	  </tr>
	  </tbody>
	</table>
	
6. 用 CSS 给table加上边框线 <pre> \<style type="text/css">
		table tr td,th{border:1px solid #111;}
	\</style>
</pre>
7. 给 table 加上摘要 <code>\<table summary="表格简介文本"></code>
8. 给 table 加上标题 <code>\<caption>标题文本\</caption></code>

### 7.各种标签————第三部分
1. \<a>标签：\<a  href="目标网址"  title="鼠标滑过显示的文本">链接显示的文本\</a><br> **举个栗子🌰  **<a herf="www.baidu.com" tittle="这是百度">这是一个链接 </a> <br> ** tips： ** a href="#"，当链接为#号时，是默认当前网址。
2. 在新建浏览器窗口中打开链接：<code> \<a href="目标网址" target="_blank">click here!\</a></code>
3. 使用mailto在网页中链接Email地址:<code> \<a href="wo18919029008@163.com?subject=这是主题&body=你好，对此你有什么想法">对此影评有何感想，发送邮件给我\</a></code> <br>** 举个栗子🌰** <a herf="wo18919029008@163.com?subject=主题&body=邮件内容"> 如果有什么想告诉我的，请发邮件给我</a>
4. 在网页的制作中为使网页炫丽美观，肯定是缺少不了图片，可以使用\<img>标签来插入图片: <code> \<img src="图片地址" alt="下载失败时的替换文本" title = "提示文本"></code><br>** 举个栗子🌰 ** <img src="http://img.mukewang.com/52da54ed0001ecfa04120172.jpg" alt="下载失败啦" title="可爱的小朋友">

### 8.各种标签----第四部分-----（交互-表单提交）
1. 网站怎样与用户进行交互？答案是使用HTML表单(form)。表单是可以把浏览者输入的数据传送到服务器端，这样服务器端程序就可以处理表单传过来的数据。语法：<code> \<form   method="传送方式"   action="服务器文件"> </code><br>** 讲解： ** <pre>
1.\<form> ：\<form>标签是成对出现的，以\<form>开始，以\</form>结束。
2.action ：浏览者输入的数据被传送到的地方,比如一个PHP页面(save.php)。
3.method ： 数据传送的方式（get/post）。
\<form    method="post"   action="save.php">
        \<label for="username">用户名:</label>
        \<input type="text" name="username" />
        \<label for="pass">密码:</label>
        \<input type="password" name="pass" />
\</form>
注意:
1、所有表单控件（文本框、文本域、按钮、单选框、复选框等）都必须放在 \<form>\</form> 标签之间（否则用户输入的信息可提交不到服务器上哦！）。
2、method : post/get 的区别这一部分内容属于后端程序员考虑的问题。
</pre>
**举个栗子🌰**
<form method="post" action="save.php">
	<label for="username">用户名：</label>
	<input type="text" name="username" />
	<label for="pass">密码：<label/>
	<input type="password" name="pass"><br /><br />
2. 当用户要在表单中键入字母、数字等内容时，就会用到文本输入框。文本框也可以转化为密码输入框。<br />
**语法：**<pre>\<form>
   \<input type="text/password" name="名称" value="文本" />
\</form>
1、type：
   当type="text"时，输入框为文本输入框;
   当type="password"时, 输入框为密码输入框。
2、name：为文本框命名，以备后台程序ASP 、PHP使用。
3、value：为文本输入框设置默认值。(一般起到提示作用)
</pre>
3. 当用户需要在表单中输入大段文字时，需要用到文本输入域。<br />
** 语法 :** <code>\<textarea  rows="行数" cols="列数">文本</textarea></code><br />
** 举个栗子🌰 **<br>
<textarea rows="10" cols="30">这是文本框</textarea>
4. 使用单选框、复选框让用户选择 <br />**语法：** <code>\<input   type="radio/checkbox"   value="值"    name="名称"   checked="checked"/></code> <br /><pre>
1、type
	当 type="radio" 时，控件为单选框  
	当 type="checkbox" 时，控件为复选框
2、value：提交数据到服务器的值（后台程序PHP使用）
3、name：为控件命名，以备后台程序 ASP、PHP 使用
4、checked：当设置 checked="checked" 时，该选项被默认选中</pre>
** 单选框的例子🌰 ** <br />
<input type="radio" value="1" name="fruit" checked="checked"> 苹果</input><br />
<input type="radio" value="2" name="fruit" > 香蕉</input><br />
<input type="radio" value="3" name="fruit" > 菠萝</input><br />
** 复选框的例子🌰 ** <br />
<input type="checkbox" value="1" name="fruit" checked="checked"> 苹果</input><br />
<input type="checkbox" value="2" name="fruit" > 香蕉</input><br />
<input type="checkbox" value="3" name="fruit" > 菠萝</input><br /><br />
5. 下拉列表框<br />
** 语法 ** <pre> 
\<form action="save.php" method="post" >
    \<label>爱好:\</label>
    \<select>
      \<option value="看书">看书\</option>
      \<option value="旅游" selected="selected">旅游\</option>
      \<option value="运动">运动\</option>
      \<option value="购物">购物\</option>
    \</select>
\</form>
</pre> 
** 说明 ** <br />value:像服务器提交的值<br />
selected：默认选择的值<br />
** 举个栗子🌰 ** <br>
<form action="save.php" method="post" >
 <label>爱好:</label>
 <select>
   <option value="看书">看书</option>
   <option value="旅游" selected="selected">旅游</option>
   <option value="运动">运动</option>
   <option value="购物">购物</option>
 </select>
</form> <br />

6. 下拉框的多选:摁住command键实现多选<br />
** 语法 ** <pre> 
\<form action="save.php" method="post" >
    \<label>爱好:\</label>
    \<select mutiple="mutiple">
      \<option value="看书">看书\</option>
      \<option value="旅游" selected="selected">旅游\</option>
      \<option value="运动">运动\</option>
      \<option value="购物">购物\</option>
    \</select>
\</form>
</pre> 
** 说明 ** <br />value:像服务器提交的值<br />
selected：默认选择的值<br />
** 举个栗子🌰 ** <br>
<form action="save.php" method="post" >
 <label>爱好:</label>
 <select multiple="multiple">
   <option value="看书">看书</option>
   <option value="旅游" selected="selected">旅游</option>
   <option value="运动">运动</option>
   <option value="购物">购物</option>
 </select>
</form> <br />

7. 使用提交按钮，提交数据<br />
** 语法 : ** <code>\<input   type="submit"   value="提交"></code><br />type：只有当type值设置为submit时，按钮才有提交作用<br />value：按钮上显示的文字<pre>
\<form action="save.php" method="post" >
	  用户名：
      \<input type="text" value="" name="myname">
	  \<input type="submit" value="提交">
\</form>
</pre>
 ** 举个栗子 **
 <form action="save.php" method="post" >
   用户名：
   <input type="text" value="" name="myname">
   <input type="submit" value="提交">
</form>
8. 重置表单：<br />
** 语法 : ** <code>\<input   type="reset"   value="提交"></code><br />type：只有当type值设置为reset时，按钮才有重置作用<br />value：按钮上显示的文字<pre>
\<form action="save.php" method="post" >
	  用户名：
      \<input type="text" value="" name="myname">
	  \<input type="reset" value="提交">
\</form>
</pre>
 ** 举个栗子 **
 <form action="save.php" method="post" >
   用户名：
   <input type="text" value="" name="myname">
   <input type="reset" value="重置">
</form>

9. form表单中的label标签：label标签不会向用户呈现任何特殊效果，它的作用是为鼠标用户改进了可用性。如果你在 label 标签内点击文本，就会触发此控件。就是说，当用户单击选中该label标签时，浏览器就会自动将焦点转到和标签相关的表单控件上（就自动选中和该label标签相关连的表单控件上）。<br />
** 语法 : ** <code>\<label for="控件id名称"></code><br />
** 举个栗子 **
 <form>
   <label for="male">男</label>
  <input type="radio" name="gender" id="male" />
  <br />
  <label for="female">女</label>
  <input type="radio" name="gender" id="female" />
  <br />
  <label for="email">输入你的邮箱地址</label>
  <input type="email" id="email" placeholder="Enter email">  
</form>
<form>
<label>你对什么运动感兴趣: </label>
<br/>
<label for="run">慢跑<label>
<input type="checkbox" name="name" id="run">
<br/>
<label for="moutain">登山<label>
<input type="checkbox" name="name" id="moutain">
<br/>
<label for="boll">篮球<label>
<input type="checkbox" name="name" id="boll">
</form>












