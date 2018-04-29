#1. introduction of web development

#2. introduction of chrome development tools
常用功能： </br>
*元素（Elements）*：用于查看或修改HTML元素的属性、CSS属性、监听事件、断点等。 </br>
*控制台（Console）*：控制台一般用于执行一次性代码，查看JavaScript对象，查看调试日志信息或异常信息。</br>
*源代码（Sources）*：该页面用于查看页面的HTML文件源代码、JavaScript源代码、CSS源代码，此外最重要的是可以调试JavaScript源代码，可以给JS代码添加断点等。</br>
*网络（Network）*：网络页面主要用于查看header等与网络连接相关的信息。</br>

引自：https://blog.csdn.net/csdnligao/article/details/53925094

#3. notes of some html labels
>##<img >
>>+ it has attribute of src="", and also alt="", besides width="", height="" or style="" or usemap=""
>>+ style="" attributes 
>>+ very interesting is src seems to be URL which means a web address.
>>+ Always specify the width and height of an image. If width and height are not specified, the page might flicker while the image loads.
>>+ It is suggested that using the style attribute. It prevents styles sheets from changing the size of images:
>>+ `<img src="html5.gif" alt="HTML5 Icon" width="128" height="128">`
>>+ `<img src="html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">`
>>### some cases about src="" attribute:
>>1. case1: images in another folder. - By default, the browser expects to find the image in the same folder as the web page. 
If not, we need to give the whole path, either absolute or relative.

>>2. case2: Images on Another Server - We need to give the address of the server like "https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com"

>>3. case3: Images on your own local PC - I don't konw right now???????

>##<map>
  >>+ the attribute is name=""
  >>+ have some sub tags ofj <area> like: <area shape="" coords="" alt="" href=""> 
  >>+ the name of the <map> is associated with the <img>'s usemap attribute 

>## <body style="background-image:url('www.baidu.jpg')">
  >>+ the attribute style="background-image:url('')" is the key
  >>+ 

>##<picture>
  >>+ The <picture> element contains a number of <source> elements, each referring to different image sources. This way the browser can choose the image that best fit the current view and/or device.
  >>+ Each <source> element have attributes describing when their image is the most suitable.
  >>+ The browser will use the first <source> element with matching attribute values, and ignore any following <source> elements.
  
**summary**

| Tag	 | Description |
|-:|:-:|
| &lt; img &gt;	| Defines an image |
| &lt; map &gt;	| Defines an image-map |
| &lt; area &gt;| Defines a clickable area inside an image-map |
| &lt; picture &gt;| Defines a container for multiple image resources |
  
<table>
  <tr>
    <th>Attribute</th>
    <th>Exemple</th>
  </tr>
  
  <tr>
    <td >src=""</td>
    <td ></td>
  </tr>
  
  <tr>
    <td >alt=""</td>
    <td ></td>
  </tr>
  <tr>
    <td > usemap=""</td>
    <td > &lt;   img usemap="#workmap"   &gt; </td>
  </tr> 
  <tr>
    <td > name=""</td>
    <td > &lt; map name="workmap" &gt; </td>
  </tr> 
   <tr>
     <td>shape=""</td>
     <td> &lt; area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm" &gt; </td>
   </tr>
   <tr>
    <td>coords=""</td>
    <td> &lt; area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm" &gt; </td>
   </tr> 
  
  <tr>
    <td rowspan="4" >style=""</td>
    <td >background-image:url('')</td>
  </tr>
    
  <tr>
    <td> width:50px </td>
  </tr>
  
  <tr>
    <td>height:100px</td>
  </tr>
  
   <tr>
    <td>float:right </td>
   </tr>
   
  
</table>
