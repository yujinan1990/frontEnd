# 1. FAQ:
- HTML是什么，HTML5是什么？ <br>

> HTML is the standard markup language for creating Web pages.
>> a. HTML stands for Hyper Text Markup Language <br>
>> b. HTML describes the structure of Web pages using markup <br>
>> c. HTML elements are the building blocks of HTML pages<br>
>> d. HTML elements are represented by tags<br>
>> e. HTML tags label pieces of content such as "heading", "paragraph", "table", and so on<br>
>> f. Browsers do not display the HTML tags, but use them to render the content of the page<br>

> HTML5 is the latest Revision. The purpose of designing it is for the support of multi-media on mobile devices.<br>
>> Some new HTML5 elements are:<br>
>> a. New semantic elements like &lt;header&gt;, &lt;footer &gt;, &lt;article&gt;, and &lt;section&gt;.<br>
>> b. New attributes of form elements like number, date, time, calendar, and range.<br>
>> c. New graphic elements: &lt;svg&gt; and &lt;canvas&gt;.<br>
>> d. New multimedia elements: &lt;audio&gt; and &lt;video&gt;.<br>
>> Some new HTML5 APIs are: <br>
>> a. HTML Drag and Drop<br>
>> b. HTML Local Storage<br>
>> c. HTML Application Cache<br>
>> d. HTML Web Workers<br>
>> e. HTML SSE<br>
>> f. HTML Geolocation<br>

- HTML元素标签、属性都是什么概念？<br>
> HTML DOCUMENT:
>> All HTML documents must start with a document type declaration:&lt;!DOCTYPE html&gt;. <br>
>> The HTML document itself begins with <html> and ends with &lt;/html&gt;.<br>
>> Only the content inside the <body> section (the white area above) is displayed in a browser. == The visible part of the HTML document is between &lt;body&gt; and &lt;/body&gt;.<br> 

> HTML ELEMENT : <br>
> An HTML element usually consists of a start tag and end tag, with the content inserted in between:
&lt;tagname &gt;Content goes here...&lt;/tagname&gt; <br>
>> The HTML element is everything from the start tag to the end tag: <br>
>> All HTML documents consist of nested HTML elements.<br>

> HTML TAG: <br> HTML tags are element names surrounded by angle brackets:
>> HTML tags normally come in pairs like &lt;p&gt; and &lt; /p &gt; <br>
>> The first tag in a pair is the start/opening tag, the second tag is the end/closing tag <br>
>> The browser does not display the HTML tags, but uses them to determine how to display the document:<br>

> HTML ATTRIBUTES: <br> Attributes provide additional information about HTML elements.<br>
>> Attributes are always specified in the start tag.<br>
>> Attributes usually come in name/value pairs like: name="value"<br>
>> *href* Specifies the URL (web address) for a link; *src*Specifies the URL (web address) for an image<br>
>> some attributes:
>>> &lt;html  lang="en-US" &gt; &lt;html&gt; Declaring a language is important for accessibility applications (screen readers) and searchengines:<br>
>>> &lt;img src="" alt="" &gt; The alt attribute specifies an alternative text to be used, when an image cannot be displayed, which can be read by screen readers;<br>
>>> &lt;p title="" &gt; &lt;/p&gt; The value of the title attribute will be displayed as a tooltip when you mouse over the paragraph:<br>

- 文档类型是什么概念，起什么作用？<br>
> The <!DOCTYPE>  is not a TAG, it is a declaration which represents the document type.
> The reson we should declare the document type is that it helps browsers to display web pages correctly regards different type like html xhtml and their different versions..  <br>
> It must only appear once, at the top of the page (before any HTML tags). <br>
> The <!DOCTYPE> declaration is not case sensitive. <br>
> The <!DOCTYPE> declaration for HTML5 is: <br>
>> &lt; !DOCTYPE html &gt; <br>

- meta标签都用来做什么的？<br>
> Describe metadata within an HTML document: <br>
> Metadata is data (information) about data.<br>
> The &lt; meta &gt; tag provides metadata about the HTML document. Metadata will not be displayed on the page, but will be machine parsable.<br>
> Meta elements are typically used to specify page description, keywords, author of the document, last modified, and other metadata.<br>
> The metadata can be used by browsers (how to display content or reload page), search engines (keywords), or other web services.<br>
> HTML5 introduced a method to let web designers take control over the viewport (the user's visible area of a web page), through the <meta> tag (See "Setting The Viewport" example below).<br>
>> &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt; <br>
>>　The width=device-width part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).<br>
>>　The initial-scale=1.0 part sets the initial zoom level when the page is first loaded by the browser.<br>
- Web语义化是什么，是为了解决什么问题 <br>
> 
- 链接是什么概念，对应什么标签？ <br>
> HTML links are hyperlinks.  You can click on a link and jump to another document.<br>
> When you move the mouse over a link, the mouse arrow will turn into a little hand.<br>
> Note: A link does not have to be text. It can be an image or any other HTML element.<br>
>some notes about the *href* value<br>
>> Without a forward slash on subfolder addresses, you might generate two requests to the server. Many servers will automatically add a forward slash to the address, and then create a new request.<br>
>> A local link (link to the same web site) is specified with a relative URL (without http://www....).<br>
> The *target* attribute can have one of the following values:<br>
>> _blank - Opens the linked document in a *new window or tab*<br>
>> _self - Opens the linked document in the *same window/tab* as it was clicked (this is default)<br>
>> _parent - Opens the linked document in the *parent frame*<br>
>> _top - Opens the linked document in the *full body of the window*<br>
>> framename - Opens the linked document in a *named frame* <br>

- 常用标签都有哪些，都适合用在什么场景 <br>
> https://websitesetup.org/wp-content/uploads/2014/09/html5-cheat-sheet.png
- 表单标签都有哪些，对应着什么功能，都有哪些属性<br>
> The HTML &lt; form &gt; element defines a form that is used to collect user input: <br>
>　It contains form elements.　Form elements are different types of input elements, like text fields, checkboxes, radio buttons, submit buttons, and more. <br>
>> the attributes of &lt; form &gt;:
>> The *action* attribute defines the action to be performed when the form is submitted. Normally, the form data is sent to a web page(contains a server-side script that handles the form data) on the server when the user clicks on the submit button.<br>
>> The *target* attribute  specifies if the submitted result will open in a new browser tab, a frame, or in the current window.<br>
>> The *method* attribute specifies the HTTP method (GET or POST) to be used when submitting the form data:<br>
>>> Notes on GET:
>>>+ Appends form-data into the URL in name/value pairs<br>
>>>+ The length of a URL is limited (about 3000 characters)<br>
>>>+ Never use GET to send sensitive data! (will be visible in the URL)<br>
>>>+ Useful for form submissions where a user want to bookmark the result<br>
>>>+ GET is better for non-secure data, like query strings in Google<br><br>

>>> Notes on PUT:
>>>+ POST has no size limitations, and can be used to send large amounts of data.<br>
>>>+ Form submissions with POST cannot be bookmarked <br>
> The &lt; input &gt; element is the most important form element.The &lt; input &gt; element can be displayed in several ways, depending on the type attribute. <br>
>> the attributes of &lt; input &gt;
>>> Each input field must have a name attribute to be submitted. If the name attribute is omitted, the data of that input field will not be sent at all.
>>> 

- ol, ul, li, dl, dd, dt等这些标签都适合用在什么地方，举个例子<br>
>



