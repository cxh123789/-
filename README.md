# 学习知识点整理
## HTML、CSS

1、transform（改变）CSS3动画<br>
   用法示例
   transform:tanslateY(-50%);
   /* 选择的内容上移50%*/<br>
2、设置字体 font-family："字体"；<br>
3、设置大写 text-transform:uppercase;<br>
4、边框圆角 border-radius:**px; <br>
5、去吃a标签的下划线 text=decoration:none; <br>
6、相对定位 position：relative；
7、语言代码 
```html
<html lang="en">英文，fr法文，zh-CN中文
```
8、离线缓存<br>
优势：离线浏览、加载速度快、减少服务器负载；(注意IE，不支持！！！)<br>
用法：
```html
  <html manifest = "demo.appchche">
  文件的写法
  CACHE MANIFEST
  #修改事件：
  CACHE
  缓存文件
  NETWORK
  永不缓存文件
  FALLBACK
  页面无连接回退的页面
```
##### 注意：manifest文件主要适用于不依赖于网络，且下载后不需要更新的html5游戏、应用或者页面。
9、favicon图标
```
引用方式<link rel = "shortcut icon" type ="image/ico" href="地址">
代表网站标识也就是logo，就是选项卡最前头图标
```
10、``` <base>```是文档的基础的URL地址，例如文档中的a的值为01.html实际访问的地址是base的加上a的值。<br>
``` <base target="_blank">```可设置全局浏览器的打开方式。<br>
#### 11、```标签<meta>```
①meta规定必须包含 name（元数据名称），http-equiv(编译指令)，和charset（字符编码）其中的一种。
②标识内核使用方式 
```
<meta namr ="renderer" content="webkit">其中conten他可以设置为 ie-comp（兼容）、ie-stand(标准)。主要为了适应国内什么三核什么双核浏览器
```
③使用最新的引擎渲染
```
<meta http-equiv="X-UA-Compatible" contten="IE=edge chrome=1" >
```
④SEO优化
```
<meta name="keywords" content="关键词">
<meta name="description" content="描述">
<meta name="robts" content="none">禁止抓取
<meta namr="robts" content="all">希望抓取
<meta namr="HandheldFriendly"content="true">老式手持设备优化
<meta http-equiv="Cache-control" content="no-siteapp">禁止百度转码
<meta http-equiv="eapires" content="web 时间时区">设置缓存过期时间
```
12、article元素<br>
```<article>```作为页面中某一个独立的成分和部位，它还能够含有header和footer或者section <br>
13、侧边栏区域可以用 ``` <aside>```来标识<br>
14、```<figure>```元素，主要被用于展示插图，图表、照片、代码、用法如下
```
<figure>
  <img src="shili.png" alt="示例图片" title="对示例图片的解释说明">
  <figcaption>图片名：图片介绍</figcption>
</figure>
```
15、一个页面只能有一个main元素。<br>
**16、内容分组元素，包括p、div、ul、ol、li、dl、dt、dd、figure、main、 <br>
 语义化块元素header、section、article、asise、footer、h1、**<br>
17、input placeholder占位符，required必填,设置name="date"在桌面浏览器中能直接选择时间<br>
18、fieldset被用来对表单内容的一部分进行打包，生成一组相表单的字段。
``` 
用法
<fieldset>
  <legend>性别</legend>
  <p><label><input type="radio" name="sex"checked>男</label><p>
  <p><label><input type="radio" name="sex">女</label><p>
</fieldset>
```
19、表格，
```
<table>
  <tr>
    <th></th>
    <th></th>
  </tr>
  <tr>
    <td></td>
  <tr>
</table>
colspan跨列合并
rowspan跨行合并
caption表格的标题
<thead><tbody><tfoot>表头和主体表尾
```
20、WAI-ARIA 无障碍网页应用技术 可以添加role属性
## css
1、写宽度的时候四个值分别代表上右下左顺时针<br>
2、写百分比的时候值为0的时候不可以写0要写0%<br>
3、在CSS中是一种重要基本特性。如果为了避免默认浏览器设置的影响，我们常常使用专门的css重设文件。<br>
4、css中存在三种种主要的选择器。标签、类、id <br>
5、伪类是在之前的选择器的基础上，加上一些用于指定元素状态的关键字，如鼠标位置。标志是在选择器和关键字之间加冒号。如已经访问visited。
```
例如在某段文字💰加文字
<p>这前面<p>
p::before{
    content:"kk";
}
```
6、文字粗细 font-weight， normal和bold值<br>
7、em代表页面一个字符大小的基准值，h1默认的大小值为2em<br>
8、文本缩进 text-indent。单位最好为em因为按字符缩进啊<br>
9、行高 line-height<br>
**10、CSS中line-heighth
## JavaScript
1、点击事件onclick <br>
```javascript
var roll = document.getElementById("roll");
rool.onclick = function(){
    roll.innerHTML = "点击完成"；
    roll.style = "background-coloe:blue"
}
```
