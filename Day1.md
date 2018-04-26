#1. introduction of web development

#2. introduction of chrome development tools

#3. notes of some html labels
>##<img >
>>+ it has attribute of src="", and also alt="", besides width="", height="" or style="".
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
  
>##<picture>
