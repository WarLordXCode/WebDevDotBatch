# WebDevDotBatch
Full Stack Web Development

# HTML Basics

<br/>
## Table of Contents

* [Introduction](#-1-introduction)
* [HTML Tags](#-2-html-tags)
* [HTML Events](#-3-html-events)
* [HTML Forms](#-4-html-forms)
* [HTML Tables](#-5-html-tables)
* [HTML Lists](#-6-html-lists)
* [HTML Iframe](#-6-html-iframe)
* [HTML URL](#-6-html-url)
* [HTML SVG](#-7-html-svg)
* [HTML Canvas](#-8-html-canvas)
* [HTML Storage](#-9-html-storage)
* [HTML APIs](#-10-html-apis)
* [HTML Drag and Drop](#-11-html-drag-and-drop)
* [HTML Web Worker](#-12-html-web-worker)
* [HTML Accessibility](#-13-html-accessibility)
* [Miscellaneous](#-14-miscellaneous)

<br/>

## # 1. Introduction

<br/>

## Q. What is difference between HTML and XHTML?

The Extensible Hypertext Markup Language, or XHTML, has two important notes for front end developers.

1) It needs to be well formed, meaning all elements need to be closed and nested correctly or you will return errors.
2) Since it is more strict than HTML is requires less pre-processing by the browser, which may improve your sites performance.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>


## Q. What does a `<DOCTYPE html>` do?

A DOCTYPE is always associated to a `DTD` ( **Document Type Definition** ). A DTD defines how documents of a certain type should be structured (i.e. a `button` can contain a `span` but not a `div`), whereas a DOCTYPE declares what DTD a document supposedly respects (i.e. this document respects the HTML DTD). For webpages, the DOCTYPE declaration is required. It is used to tell user agents what version of the HTML specifications your document respects. 

Once a user agent has recognized a correct DOCTYPE, it will trigger the `no-quirks mode` matching this DOCTYPE forreading the document. If a user agent doesn't recognize a correct DOCTYPE, it will trigger the `quirks mode`.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What happens when DOCTYPE is not given?

The web page is rendered in quirks mode. The web browsers engines use quirks mode to support older browsers which does not follow the **W3C specifications**. In quirks mode CSS class and id names are case insensitive. In standards mode they are case sensitive.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the new form elements in HTML5?

There are five new form elements in the HTML5 forms specification: `<datalist>`, `<output>`, `<progress>`, and `<meter>`. 


## Q. What are the semantic tags available in html5?

HTML5 semantic tags define the function and the category of your text, simplifying the work for browsers and search engines, as well as developers.

HTML5 offers new semantic elements to define different parts of a web page:

* `<article>`
* `<aside>`
* `<details>`
* `<figcaption>`
* `<figure>`
* `<footer>`
* `<header>`
* `<main>`
* `<mark>`
* `<nav>`
* `<section>`
* `<summary>`
* `<time>`

**Syntax:**

```html
<!DOCTYPE html> 

<html>  
   <head> 
      <meta charset = "utf-8"/> 
      <title>...</title> 
   </head> 
  
   <body> 
      <header>...</header> 
      <nav>...</nav> 
      
      <article> 
         <section> 
            ... 
         </section> 
      </article> 
      <aside>...</aside> 
      
      <footer>...</footer> 
   </body> 
</html> 
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Why you would like to use semantic tag?

* Search Engine Optimization, accessibility, repurposing, light code. 
* Many visually impaired person rely on browser speech and semantic tag helps to interpret page content clearly.
* Search engine needs to understand page content to rank and semantic tag helps.
* Semantic code aids accessibility. Specially, many people whose eyes are not good rely on speech browsers to read pages to them. These programs cannot interpret pages very well unless they are clearly explained.
* Help Search engines to better understand pages. Search engine need to understand what your content is about when rank you properly on search engines. Semantic code tends to improve your placement on search engines, as it is easier for the "search engine spiders" to understand.
* It\'s easier to read and edit, which saves time and money during maintenance.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>



## HTML5 Tags

#### Structural Tags

|Tag	            |Description                                            |
|-------------------|-------------------------------------------------------|
|`<a>`	            |Defines a hyperlink.|
|`<article>` 	    |Defines an article.|
|`<aside>` 	        |Defines some content loosely related to the page content.|
|`<body>`	        |Defines the document's body.|
|`<br>`	            |Produces a single line break.|
|`<details>` 	    |Represents a widget from which the user can obtain additional information or controls on-demand.|
|`<div>`	        |Specifies a division or a section in a document.|
|`<h1>` to `<h6>`	|Defines HTML headings.|
|`<head>`	        |Defines the head portion of the document that contains information about the document.|
|`<header>` 	    |Represents the header of a document or a section.|
|`<hgroup>` 	    |Defines a group of headings.|
|`<hr>`	            |Produce a horizontal line.|
|`<html>`	        |Defines the root of an HTML document.|
|`<footer>` 	    |Represents the footer of a document or a section.|
|`<nav>` 	        |Defines a section of navigation links.|
|`<p>`	            |Defines a paragraph.|
|`<section>` 	    |Defines a section of a document, such as header, footer etc.|
|`<span>`	        |Defines an inline styleless section in a document.|
|`<summary>` 	    |Defines a summary for the `<details>` element.|

#### Metadata Tags

|Tag	            |Description                                          |
|-------------------|-----------------------------------------------------|
|`<base>`	        |Defines the base URL for all linked objects on a page.|
|`<link>`	        |Defines the relationship between the current document and an external resource.||
|`<meta>`	        |Provides structured metadata about the document content.|
|`<style>`	        |Inserts style information (commonly CSS) into the head of a document.|
|`<title>`	        |Defines a title for the document.|


#### Form Tags

|Tag	         |Description                                                    |
|----------------|---------------------------------------------------------------|
|`<button>`	     |Creates a clickable button.|
|`<datalist>` 	 |Represents a set of pre-defined options for an `<input>` element.|
|`<fieldset>`	 |Specifies a set of related form fields.|
|`<form>`	     |Defines an HTML form for user input.|
|`<input>`	     |Defines an input control.|
|`<keygen>` 	 |Represents a control for generating a public-private key pair.|
|`<label>`	     |Defines a label for an `<input>` control.|
|`<legend>`	     |Defines a caption for a `<fieldset>` element.|
|`<meter>` 	     |Represents a scalar measurement within a known range.|
|`<optgroup>`	 |Defines a group of related options in a selection list.|
|`<option>`	     |Defines an option in a selection list.|
|`<select>`	     |Defines a selection list within a form.|
|`<textarea>`	 |Defines a multi-line text input control (text area).|


#### Formatting Tags


|Tag	          |Description                                            |
|-----------------|-------------------------------------------------------|
|`<abbr>`	      |Defines an abbreviated form of a longer word or phrase.|
|`<acronym>`      |Defines an acronym.|
|`<address>`	  |Specifies the author's contact information.|
|`<b>`	          |Displays text in a bold style.|
|`<bdi>` 	      |Represents text that is isolated from its surrounding for the purposes of bidirectional text formatting.|
|`<bdo>`	      |Overrides the current text direction.|
|`<big>`	      |displays text in a large size.|
|`<blockquote>`	  |Defines a long quotation.|
|`<cite>`	      |Indicates a citation or reference to another source.|
|`<code>`	      |Specifies text as computer code.|
|`<del>`	      |Specifies a block of deleted text.|
|`<dfn>`	      |Specifies a definition.|
|`<em>`	          |Specifies emphasized text.|
|`<i>`	          |Displays text in an italic style.|
|`<ins>`	      |Defines a block of text that has been inserted into a document.|
|`<kbd>`	      |Specifies text as keyboard input.|
|`<mark>` 	      |Represents text highlighted for reference purposes.|
|`<output>` 	  |Represents the result of a calculation.|
|`<pre>`	      |Defines a block of preformatted text.|
|`<progress>` 	  |Represents the completion progress of a task.|
|`<q>`	          |Defines a short inline quotation.|
|`<rp>` 	      |Provides fall-back parenthesis for browsers that don't support ruby annotations.|
|`<rt>` 	      |Defines the pronunciation of character presented in a ruby annotations.|
|`<ruby>` 	      |Represents a ruby annotation.|
|`<samp>`	      |Specifies text as sample output from a computer program.|
|`<small>`	      |Displays text in a smaller size.|
|`<strong>`	      |Indicate strongly emphasized text.|
|`<sub>`	      |Defines subscripted text.|
|`<sup>`	      |Defines superscripted text.|
|`<tt>`	          |Displays text in a teletype style.|
|`<var>`	      |Defines a variable.|
|`<wbr>` 	      |Represents a line break opportunity.|



#### List Tags

|Tag	         |Description                                            |
|----------------|-------------------------------------------------------|
|`<dd>`	         |Specifies a definition for a term in a definition list.|
|`<dl>`	         |Defines a definition list.|
|`<dt>`	         |Defines a term (an item) in a definition list.|
|`<li>`	         |Defines a list item.|
|`<ol>`	         |Defines an ordered list.|
|`<menu>`	     |Represents a list of commands.|
|`<ul>`	         |Defines an unordered list.|


#### Table Tags


|Tag	          |Description|
|-----------------|-------------------------------------------------------|
|`<caption>`	  |Defines the title of a table.|
|`<col>`	      |Defines attribute values for one or more columns in a table.|
|`<colgroup>`	  |Specifies attributes for multiple columns in a table.|
|`<table>`	      |Defines a data table.|
|`<tbody>`	      |Groups a set of rows defining the main body of the table data.|
|`<td>`	          |Defines a cell in a table.|
|`<tfoot>`	      |Groups a set of rows summarizing the columns of the table.|
|`<thead>`	      |Groups a set of rows that describes the column labels of a table.|
|`<th>`	          |Defines a header cell in a table.|
|`<tr>`	          |Defines a row of cells in a table.|


#### Scripting Tags

|Tag	          |Description                                                                       |
|-----------------|----------------------------------------------------------------------------------|
|`<noscript>`	  |Defines alternative content to display when the browser doesn't support scripting.|
|`<script>`	      |Places script in the document for client-side processing.|


#### Embedded Content Tags

|Tag	          |Description                                                                                   |
|-----------------|----------------------------------------------------------------------------------------------|
|`<area>`	      |Defines a specific area within an image map.|
|`<audio>` 	      |Embeds a sound, or an audio stream in an HTML document.|
|`<canvas>` 	  |Defines a region in the document, which can be used to draw graphics on the fly via scripting (usually JavaScript).|
|`<embed>` 	      |Embeds external application, typically multimedia content like audio or video into an HTML document.|
|`<figcaption>`   |Defines a caption or legend for a figure.|
|`<figure>` 	  |Represents a figure illustrated as part of the document.|
|`<frame>`	      |Defines a single frame within a frameset.|
|`<frameset>`	  |Defines a collection of frames or other frameset.|
|`<iframe>`	      |Displays a URL in an inline frame.|
|`<img>`	      |Displays an inline image.|
|`<map>`	      |Defines a client-side image-map.|
|`<noframes>`	  |Defines an alternate content that displays in browsers that do not support frames.|
|`<object>`	      |Defines an embedded object.|
|`<param>`	      |Defines a parameter for an object or applet element.|
|`<source>` 	  |Defines alternative media resources for the media elements like `<audio>` or `<video>`.|
|`<time>` 	      |Represents a time and/or date.|
|`<video>` 	      |Embeds video content in an HTML document.|





## HTML5 Events List

|Sl.No|Event                |Description                                         |
|-----|---------------------|----------------------------------------------------|
| 01. |offline				|Triggers when the document goes offline|
| 02. |onabort				|Triggers on an abort event|
| 03. |onafterprint		|Triggers after the document is printed|
| 04. |onbeforeonload		|Triggers before the document loads|
| 05. |onbeforeprint		|Triggers before the document is printed|
| 06. |onblur				|Triggers when the window loses focus|
| 07. |oncanplay			|Triggers when media can start play, but might has to stop for buffering|
| 08. |oncanplaythrough	|Triggers when media can be played to the end, without stopping for buffering|
| 09. |onchange			|Triggers when an element changes|
| 10. |onclick				|Triggers on a mouse click|
| 11. |oncontextmenu		|Triggers when a context menu is triggered|
| 12. |ondblclick			|Triggers on a mouse double-click|
| 13. |ondrag				|Triggers when an element is dragged|
| 14. |ondragend			|Triggers at the end of a drag operation|
| 15. |ondragenter			|Triggers when an element has been dragged to a valid drop target|
| 16. |ondragleave			|Triggers when an element leaves a valid drop target|
| 17. |ondragover			|Triggers when an element is being dragged over a valid drop target|
| 18. |ondragstart			|Triggers at the start of a drag operation|
| 19. |ondrop				|Triggers when dragged element is being dropped|
| 20. |ondurationchange	|Triggers when the length of the media is changed|
| 21. |onemptied			|Triggers when a media resource element suddenly becomes empty.|
| 22. |onended				|Triggers when media has reach the end|
| 23. |onerror				|Triggers when an error occur|
| 24. |onfocus				|Triggers when the window gets focus|
| 25. |onformchange		|Triggers when a form changes|
| 26. |onforminput			|Triggers when a form gets user input|
| 27. |onhaschange			|Triggers when the document has change|
| 28. |oninput				|Triggers when an element gets user input|
| 29. |oninvalid			|Triggers when an element is invalid|
| 30. |onkeydown			|Triggers when a key is pressed|
| 31. |onkeypress			|Triggers when a key is pressed and released|
| 32. |onkeyup				|Triggers when a key is released|
| 33. |onload				|Triggers when the document loads|
| 34. |onloadeddata		|Triggers when media data is loaded|
| 35. |onloadedmetadata	|Triggers when the duration and other media data of a media element is loaded|
| 36. |onloadstart			|Triggers when the browser starts to load the media data|
| 37. |onmessage			|Triggers when the message is triggered|
| 38. |onmousedown			|Triggers when a mouse button is pressed|
| 39. |onmousemove			|Triggers when the mouse pointer moves|
| 40. |onmouseout			|Triggers when the mouse pointer moves out of an element|
| 41. |onmouseover			|Triggers when the mouse pointer moves over an element|
| 42. |onmouseup			|Triggers when a mouse button is released|
| 43. |onmousewheel		|Triggers when the mouse wheel is being rotated|
| 44. |onoffline			|Triggers when the document goes offline|
| 45. |ononline			|Triggers when the document comes online|
| 46. |onpagehide			|Triggers when the window is hidden|
| 47. |onpageshow			|Triggers when the window becomes visible|
| 48. |onpause				|Triggers when media data is paused|
| 49. |onplay				|Triggers when media data is going to start playing|
| 50. |onplaying			|Triggers when media data has start playing|
| 51. |onpopstate			|Triggers when the window's history changes|
| 52. |onprogress			|Triggers when the browser is fetching the media data|
| 53. |onratechange		|Triggers when the media data's playing rate has changed|
| 54. |onreadystatechange	|Triggers when the ready-state changes|
| 55. |onredo				|Triggers when the document performs a redo|
| 56. |onresize			|Triggers when the window is resized|
| 57. |onscroll			|Triggers when an element's scrollbar is being scrolled|
| 58. |onseeked			|Triggers when a media element's seeking attribute is no longer true, and the seeking has ended|
| 59. |onseeking			|Triggers when a media element's seeking attribute is true, and the seeking has begun|
| 60. |onselect			|Triggers when an element is selected|
| 61. |onstalled			|Triggers when there is an error in fetching media data|
| 62. |onstorage			|Triggers when a document loads|
| 63. |onsubmit			|Triggers when a form is submitted|
| 64. |onsuspend			|Triggers when the browser has been fetching media data, but stopped before the entire media file was fetched|
| 65. |ontimeupdate		|Triggers when media changes its playing position|
| 66. |onundo				|Triggers when a document performs an undo|
| 67. |onunload			|Triggers when the user leaves the document|
| 68. |onvolumechange		|Triggers when media changes the volume, also when volume is set to "mute"|
| 69. |onwaiting			|Triggers when media has stopped playing, but is expected to resume|
