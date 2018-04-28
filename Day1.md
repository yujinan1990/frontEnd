#1. introduction of web development

#2. introduction of chrome development tools

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
| <img>	| Defines an image |
| <map>	| Defines an image-map |
| <area>	| Defines a clickable area inside an image-map |
| <picture>	| Defines a container for multiple image resources |
  
<table>
  <tr>
    <th>Attribute</th>
    <th>Description</th>
  </tr>
  
  <tr>
    <td rowspan="5" >style=""</td>
    <td >src=""</td>
  </tr>
  <tr>
    <td >background-image:url('')</td>
  </tr>
  <tr>
    <td>width:50px</td>
  </tr>
  <tr>
    <td>height:100px</td>
  </tr>
   <tr>
    <td>alt:""</td>
   </tr>
   <tr>
    <td>shape:""</td>
   </tr>
   <tr>
    <td>coords:""</td>
   </tr> 
   <tr>
    <td>=usemap=""</td>
    <td>...</td>
  </tr>
  
</table>
