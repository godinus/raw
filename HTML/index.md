<h1 align="center"><abbr title="HTML5 index"><img src="./img/abc.webp" height="150"></abbr></h1>

[![](./img/html5_small.webp)<<< README.md](README.md)

---

**·[ - ](index.md#-)···[ A ](#a)···[ B ](#b)···[ C ](#c)···[ D ](#d)···[ E ](#e)···[ F ](#f)···[ G ](#g)···[ H ](#h)···[ I ](#i)···[ J ](#j)···[ K ](#k)···[ L ](#l)···[ M ](#m)···[ N ](#n)···[ O ](#o)···[ P ](#p)···[ Q ](#q)···[ R ](#r)···[ S ](#s)···[ T ](#t)···[ U ](#u)···[ V ](#v)···[ W ](#w)···[ X ](#x)···[ Y ](#y)···[ Z ](#z)·**

---

Attribute type|Tags / attributes
-:|-
[AREA](#area-attributes)|[`<area>`](#area), [`<textarea>`](#textarea)
[CONTAINER](#container-attributes)|[`<embed>`](#embed) [`<iframe>`](#iframe) [`<object>`](#object) [`<param>`](#param)
[DOCUMENT](#document-attributes)|[`<body>`](#body) [`<meta>`](#meta)
[FORM](#form-attributes)|[`<button>`](#button) [`<fieldset>`](#fieldset) [`<form>`](#form) [`<input>`](#input) [`<label>`](#label) [`<optgroup>`](#optgroup) [`<option>`](#option) [`<output>`](#output) [`<select>`](#select)
[FORMAT](#format-attributes)|[`<del>`](#del) [`<ins>`](#ins) [`<style>`](#style)  
[GLOBAL](#global-attributes)|Global attributes (`accesskey, class, contenteditable, data-*, dir, draggable, hidden, id, spellcheck, style, tabindex, title, translate`) can be used with all HTML elements.
[LINK (URL)](#link-url-attributes)|[`<a>`](#a) [`<base>`](#base) [`<blockquote>`](#blockquote) [`<del>`](#del) [`<ins>`](#ins) [`<link>`](#link) [`<q>`](#q) [`<source>`](#source)
[LIST](#list-attributes)|[`<li>`](#li) [`<ol>`](#ol)
[MEASUREMENT](#measurement-attributes)|[`<meter>`](#meter) [`<progress>`](#progress) [`<time>`](#time)
[MEDIA](#media-attributes)|[`<audio>`](#audio) [`<canvas>`](#canvas) [`<img>`](#img) [`<map>`](#map) [`<track>`](#track) [`<video>`](#video)
[NOT SUPPORTED](#not-supported-attributes-in-html5)|These attributes: `align, bgcolor, border, color` not supported in HTML5. Use CSS instead.
[SCRIPT](#script-attributes)|[`<script>`](#script)
[TABLE](#table-attributes)|[`<td>`](#td) [`<th>`](#th) [`<col>`](#col) [`<colgroup>`](#colgroup)
[VISIBLE ELEMENTS'](#visible-elements-attributes)|These attributes (`onblur, onchange, onclick, oncontextmenu, oncopy, oncut, ondblclick, ondrag, ondragend, ondragenter, ondragleave, ondragover, ondragstart, ondrop, onfocus, oninput, oninvalid, onkeydown, onkeypress, onkeyup, onmousedown, onmousemove, onmouseout, onmouseover, onmouseup, onmousewheel, onpaste, onscroll, onselect, onwheel`) can be used with all visible HTML elements.
[WIDGET](#widget-attributes)|[`<details>`](#details)

### AREA ATTRIBUTES
> [<<<](#)
#### `<area>`
Attribute|Description
-:|-
[alt](#alt)|_Specifies an alternate text when the original element fails to display_
[coords](#coords)|_Specifies the coordinates of the area_
[download](#download)|_Specifies that the target will be downloaded when a user clicks on the hyperlink_
[href](#href)|_Specifies the URL of the page the link goes to_
[hreflang](#hrflang)|_Specifies the language of the linked document_
[media](#media)|_Specifies what media/device the linked document is optimized for_
[rel](#rel)|_Specifies the relationship between the current document and the linked document_
[shape](#shape)|_Specifies the shape of the area_
[target](#target)|_Specifies the target for where to open the linked document or where to submit the form_

#### `<textarea>`
Attribute|Description
-:|-
autofocus|_Specifies that the element should automatically get focus when the page loads_
cols|_Specifies the visible width of a text area_
dirname|_Specifies that the text direction will be submitted_
disabled|_Specifies that the specified element/group of elements should be disabled_
form|_Specifies the name of the form the element belongs to_
maxlength|_Specifies the maximum number of characters allowed in an element_
name|_Specifies the name of the element_
placeholder|_Specifies a short hint that describes the expected value of the element_
readonly|_Specifies that the element is read-only_
required|_Specifies that the element must be filled out before submitting the form_
rows|_Specifies the visible number of lines in a text area_
wrap|_Specifies how the text in a text area is to be wrapped when submitted in a form_

### CONTAINER ATTRIBUTES
> [<<<](#)
#### `<embed>`
Attribute|Description
-:|-
height|_Specifies the height of the element_
onabort|_Script to be run on abort_
oncanplay|_Script to be run when a file is ready to start playing (when it has buffered enough to begin)_
onerror|_Script to be run when an error occurs_
src|_Specifies the URL of the media file_
type|_Specifies the type of element_
width|_Specifies the width of the element_

#### `<iframe>`
Attribute|Description
-:|-
height|_Specifies the height of the element_
name|_Specifies the name of the element_
onload|_Script to be run when the element is finished loading_
sandbox|_Enables an extra set of restrictions for the content in an \<iframe>_
src|_Specifies the URL of the media file_
srcdoc|_Specifies the HTML content of the page to show in the \<iframe>_
width|_Specifies the width of the element_

#### `<object>`
Attribute|Description
-:|-
data|_Specifies the URL of the resource to be used by the object_
form|_Specifies the name of the form the element belongs to_
height|_Specifies the height of the element_
name|Specifies the name of the element_
onabort|_Script to be run on abort_
oncanplay|_Script to be run when a file is ready to start playing (when it has buffered enough to begin)_
onerror|_Script to be run when an error occurs_
type|_Specifies the type of element_
usemap|_Specifies an image as a client-side image map_
width|_Specifies the width of the element_

#### `<param>`
Attribute|Description
-:|-
name|_Specifies the name of the element_
value|_Specifies the value of the element_

### DOCUMENT ATTRIBUTES
> [<<<](#)
#### `<body>`
Attribute|Description
-:|-
onafterprint|_Script to be run after the document is printed_
onbeforeprint|_Script to be run before the document is printed_
onbeforeunload|_Script to be run when the document is about to be unloaded_
onerror|_Script to be run when an error occurs_
onhashchange|_Script to be run when there has been changes to the anchor part of the a URL_
onload|_Script to be run when the element is finished loading_
onoffline|_Script to be run when the browser starts to work offline_
ononline|_Script to be run when the browser starts to work online_
onpagehide|_Script to be run when a user navigates away from a page_
onpageshow|_Script to be run when a user navigates to a page_
onpopstate|_Script to be run when the window's history changes_
onresize|_Script to be run when the browser window is being resized_
onstorage|_Script to be run when a Web Storage area is updated_
onunload|_Script to be run when a page has unloaded (or the browser window has been closed)_

#### `<meta>`
Attribute|Description
-:|-
charset|_Specifies the character encoding_
content|_Gives the value associated with the http-equiv or name attribute_
http-equiv|_Provides an HTTP header for the information/value of the content attribute_
name|_Specifies the name of the element_

### FORM ATTRIBUTES
> [<<<](#)
#### `<button>`
Attribute|Description
-:|-
autofocus|_Specifies that the element should automatically get focus when the page loads_
disabled|_Specifies that the specified element/group of elements should be disabled_
form|_Specifies the name of the form the element belongs to_
formaction|_Specifies where to send the form-data when a form is submitted. Only for type="submit"_
name|_Specifies the name of the element_
type|_Specifies the type of element_
value|_Specifies the value of the element_

#### `<fieldset>`
Attribute|Description
-:|-
disabled|_Specifies that the specified element/group of elements should be disabled_
form|_Specifies the name of the form the element belongs to_
name|_Specifies the name of the element_

#### `<form>`
Attribute|Description
-:|-
accept-charset|_Specifies the character encodings that are to be used for the form submission_
action|_Specifies where to send the form-data when a form is submitted_
autocomplete|_Specifies whether the \<form> or the \<input> element should have autocomplete enabled_
enctype|_Specifies how the form-data should be encoded when submitting it to the server (only for method="post")_
method|_Specifies the HTTP method to use when sending form-data_
name|_Specifies the name of the element_
novalidate|_Specifies that the form should not be validated when submitted_
onreset|_Script to be run when a reset button in a form is clicked_
onsubmit|_Script to be run when a form is submitted_
rel|_Specifies the relationship between the current document and the linked document_
target|_Specifies the target for where to open the linked document or where to submit the form_

#### `<input>`
Attribute|Description
-:|-
accept|_Specifies the types of files that the server accepts (only for type="file")_
alt|_Specifies an alternate text when the original element fails to display_
autocomplete|_Specifies whether the <form> or the \<input> element should have autocomplete enabled_
autofocus|_Specifies that the element should automatically get focus when the page loads_
checked|_Specifies that an \<input> element should be pre-selected when the page loads (for type="checkbox" or type="radio")_
dirname|_Specifies that the text direction will be submitted_
disabled|_Specifies that the specified element/group of elements should be disabled_
form|_Specifies the name of the form the element belongs to_
formaction|_Specifies where to send the form-data when a form is submitted. Only for type="submit"_
height|_Specifies the height of the element_
list|_Refers to a \<datalist> element that contains pre-defined options for an \<input> element_
max|_Specifies the maximum value_
maxlength|_Specifies the maximum number of characters allowed in an element_
min|_Specifies a minimum value_
multiple|_Specifies that a user can enter more than one value_
name|_Specifies the name of the element_
onload|_Script to be run when the element is finished loading_
onsearch|_Script to be run when the user writes something in a search field (for \<input="search">)_
pattern|_Specifies a regular expression that an \<input> element's value is checked against_
placeholder|_Specifies a short hint that describes the expected value of the element_
readonly|_Specifies that the element is read-only_
required|_Specifies that the element must be filled out before submitting the form_
src|_Specifies the URL of the media file_
size|_Specifies the width, in characters (for \<input>) or specifies the number of visible options (for \<select>)_
step|_Specifies the legal number intervals for an input field_
type|_Specifies the type of element_
value|_Specifies the value of the element_
width|_Specifies the width of the element_

#### `<label>`
Attribute|Description
-:|-
for|_Specifies which form element(s) a label/calculation is bound to_
form|_Specifies the name of the form the element belongs to_

#### `<optgroup>`
Attribute|Description
-:|-
disabled|_Specifies that the specified element/group of elements should be disabled_
label|_Specifies the title of the text track_

#### `<option>`
Attribute|Description
-:|-
disabled|_Specifies that the specified element/group of elements should be disabled_
label|_Specifies the title of the text track_
selected|_Specifies that an option should be pre-selected when the page loads_
value|_Specifies the value of the element_

#### `<output>`
Attribute|Description
-:|-
for|_Specifies which form element(s) a label/calculation is bound to_
form|_Specifies the name of the form the element belongs to_
name|_Specifies the name of the element_

#### `<select>`
Attribute|Description
-:|-
autofocus|_Specifies that the element should automatically get focus when the page loads_
disabled|_Specifies that the specified element/group of elements should be disabled_
form|_Specifies the name of the form the element belongs to_
multiple|_Specifies that a user can enter more than one value_
name|_Specifies the name of the element_
required|_Specifies that the element must be filled out before submitting the form
size|_Specifies the width, in characters (for \<input>) or specifies the number of visible options (for \<select>)

### FORMAT ATTRIBUTES
> [<<<](#)
#### `<del>`
Attribute|Description
-:|-
datetime|_Specifies the date and time_

#### `<ins>`
Attribute|Description
-:|-
datetime|_Specifies the date and time_

#### `<style>`
Attribute|Description
-:|-
media|_Specifies what media/device the linked document is optimized for_
onerror|_Script to be run when an error occurs_
onload|_Script to be run when the element is finished loading_
type|_Specifies the type of element_

### GLOBAL ATTRIBUTES
> [<<<](#)

**Global attributes can be used with all HTML elements.**
Attribute|Description
-:|-
accesskey|_Specifies a shortcut key to activate/focus an element_
class|_Specifies one or more classnames for an element (refers to a class in a style sheet)_
contenteditable|_Specifies whether the content of an element is editable or not_
data-*|_Used to store custom data private to the page or application_
dir|_Specifies the text direction for the content in an element_
draggable|_Specifies whether an element is draggable or not_
hidden|_Specifies that an element is not yet, or is no longer, relevant_
id|_Specifies a unique id for an element_
lang|_Specifies the language of the element's content_
spellcheck|_Specifies whether the element is to have its spelling and grammar checked or not_
style|_Specifies an inline CSS style for an element_
tabindex|_Specifies the tabbing order of an element_
title|_Specifies extra information about an element_
translate|_Specifies whether the content of an element should be translated or not_

### LINK (URL) ATTRIBUTES
> [<<<](#)
#### `<a>`
Attribute|Description
-:|-
download|_Specifies that the target will be downloaded when a user clicks on the hyperlink_
href|_Specifies the URL of the page the link goes to_
hreflang|_Specifies the language of the linked document_
media|_Specifies what media/device the linked document is optimized for_
rel|_Specifies the relationship between the current document and the linked document_
target|_Specifies the target for where to open the linked document or where to submit the form_
type|_Specifies the type of element_

#### `<base>`
Attribute|Description
-:|-
href|_Specifies the URL of the page the link goes to_

#### `<blockquote>`
Attribute|Description
-:|-
cite|_Specifies a URL which explains the quote/deleted/inserted text_

#### `<del>`
Attribute|Description
-:|-
cite|_Specifies a URL which explains the quote/deleted/inserted text_

#### `<ins>`
Attribute|Description
-:|-
cite|_Specifies a URL which explains the quote/deleted/inserted text_

#### `<link>`
Attribute|Description
-:|-
href|_Specifies the URL of the page the link goes to_
hreflang|_Specifies the language of the linked document_
media|_Specifies what media/device the linked document is optimized for_
rel|_Specifies the relationship between the current document and the linked document_
onload|_Script to be run when the element is finished loading_
sizes|_Specifies the size of the linked resource_
target|_Specifies the target for where to open the linked document or where to submit the form_
type|_Specifies the type of element_

#### `<q>`
Attribute|Description
-:|-
cite|_Specifies a URL which explains the quote/deleted/inserted text_

#### `<source>`
Attribute|Description
-:|-
media|_Specifies what media/device the linked document is optimized for_
sizes|_Specifies the size of the linked resource_
src|_Specifies the URL of the media file_
srcset|_Specifies the URL of the image to use in different situations_
type|_Specifies the type of element_

### LIST ATTRIBUTES
> [<<<](#)
#### `<li>`
Attribute|Description
-:|-
value|_Specifies the value of the element_

#### `<ol>`
Attribute|Description
-:|-
reversed|_Specifies that the list order should be descending (9,8,7...)_
start|_Specifies the start value of an ordered list_

### MEASUREMENT ATTRIBUTES
> [<<<](#)
#### `<meter>`
Attribute|Description
-:|-
form|_Specifies the name of the form the element belongs to_
high|_Specifies the range that is considered to be a high value_
low|_Specifies the range that is considered to be a low value_
max|_Specifies the maximum value_
min|_Specifies a minimum value_
optimum|_Specifies what value is the optimal value for the gauge_
value|_Specifies the value of the element_

#### `<progress>`
Attribute|Description
-:|-
max|_Specifies the maximum value_
value|_Specifies the value of the element_

#### `<time>`
Attribute|Description
-:|-
datetime|_Specifies the date and time

### MEDIA ATTRIBUTES
> [<<<](#)
#### `<audio>`
Attribute|Description
-:|-
autoplay|_Specifies that the audio/video will start playing as soon as it is ready_
controls|_Specifies that audio/video controls should be displayed (such as a play/pause button etc)_
loop|_Specifies that the audio/video will start over again, every time it is finished_
muted|_Specifies that the audio output of the video should be muted_
oncanplaythrough|_Script to be run when a file can be played all the way to the end without pausing for buffering_
onabort|_Script to be run on abort_
oncanplay|_Script to be run when a file is ready to start playing (when it has buffered enough to begin)_
ondurationchange|_Script to be run when the length of the media changes_
onemptied|_Script to be run when something bad happens and the file is suddenly unavailable (like unexpectedly disconnects)_
onended|_Script to be run when the media has reach the end (a useful event for messages like "thanks for listening")_
onerror|_Script to be run when an error occurs_
onloadeddata|_Script to be run when media data is loaded_
onloadedmetadata|_Script to be run when meta data (like dimensions and duration) are loaded_
onloadstart|_Script to be run just as the file begins to load before anything is actually loaded_
onpause|_Script to be run when the media is paused either by the user or programmatically_
onplay|_Script to be run when the media has started playing_
onplaying|_Script to be run when the media has started playing_
onprogress|_Script to be run when the browser is in the process of getting the media data_
onratechange|_Script to be run each time the playback rate changes (like when a user switches to a slow motion or fast forward mode)_
onseeked|_Script to be run when the seeking attribute is set to false indicating that seeking has ended_
onseeking|_Script to be run when the seeking attribute is set to true indicating that seeking is active_
onstalled|_Script to be run when the browser is unable to fetch the media data for whatever reason_
onvolumechange|_Script to be run each time the volume of a video/audio has been changed_
onwaiting|_Script to be run when the media has paused but is expected to resume (like when the media pauses to buffer more data)_
onsuspend|_Script to be run when fetching the media data is stopped before it is completely loaded for whatever reason_
ontimeupdate|_Script to be run when the playing position has changed (like when the user fast forwards to a different point in the media)_
preload|_Specifies if and how the author thinks the audio/video should be loaded when the page loads_
src|_Specifies the URL of the media file_

#### `<canvas>`
Attribute|Description
-:|-
height|_Specifies the height of the element_
width|_Specifies the width of the element_

#### `<img>`
Attribute|Description
-:|-
alt|_Specifies an alternate text when the original element fails to display_
height|_Specifies the height of the element_
ismap|_Specifies an image as a server-side image map_
onabort|_Script to be run on abort_
onerror|_Script to be run when an error occurs_
onload|_Script to be run when the element is finished loading_
sizes|Specifies the size of the linked resource
src|Specifies the URL of the media file
srcset|Specifies the URL of the image to use in different situations
usemap|_Specifies an image as a client-side image map_
width|_Specifies the width of the element_

#### `<map>`
Attribute|Description
-:|-
name|_Specifies the name of the element_

#### `<track>`
Attribute|Description
-:|-
default|_Specifies that the track is to be enabled if the user's preferences do not indicate that another track would be more appropriate_
kind|_Specifies the kind of text track_
label|_Specifies the title of the text track_
oncuechange|_Script to be run when the cue changes in a <track> element_
src|_Specifies the URL of the media file_
srclang|_Specifies the language of the track text data (required if kind="subtitles")_

#### `<video>`
Attribute|Description
-:|-
autoplay|_Specifies that the audio/video will start playing as soon as it is ready_
controls|_Specifies that audio/video controls should be displayed (such as a play/pause button etc)_
height|_Specifies the height of the element_
loop|_Specifies that the audio/video will start over again, every time it is finished_
muted|_Specifies that the audio output of the video should be muted_
oncanplaythrough|_Script to be run when a file can be played all the way to the end without pausing for buffering_
onabort|_Script to be run on abort_
oncanplay|_Script to be run when a file is ready to start playing (when it has buffered enough to begin)_
ondurationchange|_Script to be run when the length of the media changes_
onemptied|_Script to be run when something bad happens and the file is suddenly unavailable (like unexpectedly disconnects)_
onended|_Script to be run when the media has reach the end (a useful event for messages like "thanks for listening")_
onerror|_Script to be run when an error occurs_
onloadeddata|_Script to be run when media data is loaded_
onloadedmetadata|_Script to be run when meta data (like dimensions and duration) are loaded_
onloadstart|_Script to be run just as the file begins to load before anything is actually loaded_
onpause|_Script to be run when the media is paused either by the user or programmatically_
onplay|_Script to be run when the media has started playing_
onplaying|_Script to be run when the media has started playing_
onprogress|_Script to be run when the browser is in the process of getting the media data_
onratechange|_Script to be run each time the playback rate changes (like when a user switches to a slow motion or fast forward mode)_
onseeked|_Script to be run when the seeking attribute is set to false indicating that seeking has ended_
onseeking|_Script to be run when the seeking attribute is set to true indicating that seeking is active_
onstalled|_Script to be run when the browser is unable to fetch the media data for whatever reason_
onvolumechange|_Script to be run each time the volume of a video/audio has been changed_
onwaiting|_Script to be run when the media has paused but is expected to resume (like when the media pauses to buffer more data)_
onsuspend|_Script to be run when fetching the media data is stopped before it is completely loaded for whatever reason_
ontimeupdate|_Script to be run when the playing position has changed (like when the user fast forwards to a different point in the media)_
preload|_Specifies if and how the author thinks the audio/video should be loaded when the page loads_
poster|_Specifies an image to be shown while the video is downloading, or until the user hits the play button_
src|_Specifies the URL of the media file_
width|_Specifies the width of the element_

### NOT SUPPORTED ATTRIBUTES IN HTM5
> [<<<](#)
**These attributes not supported in HTML5. Use CSS instead.
Attribute|Description
-:|-
align|_Specifies the alignment according to surrounding elements. Use CSS instead_
bgcolor|_Specifies the background color of an element. Use CSS instead_
border|_Specifies the width of the border of an element. Use CSS instead_
color|_Not supported in HTML 5.	Specifies the text color of an element. Use CSS instead_

### SCRIPT ATTRIBUTES
> [<<<](#)
#### `<script>`
Attribute|Description
-:|-
async|_Specifies that the script is executed asynchronously (only for external scripts)_
charset|_Specifies the character encoding_
defer|_Specifies that the script is executed when the page has finished parsing (only for external scripts)_
onerror|_Script to be run when an error occurs_
onload|_Script to be run when the element is finished loading_
src|_Specifies the URL of the media file_
type|_Specifies the type of element_

### TABLE ATTRIBUTES
> [<<<](#)
#### `<td>`
Attribute|Description
-:|-
colspan|_Specifies the number of columns a table cell should span_
headers|_Specifies one or more headers cells a cell is related to_
rowspan|_Specifies the number of rows a table cell should span_

#### `<th>`
Attribute|Description
-:|-
colspan|_Specifies the number of columns a table cell should span_
headers|_Specifies one or more headers cells a cell is related to_
rowspan|_Specifies the number of rows a table cell should span_
scope|_Specifies whether a header cell is a header for a column, row, or group of columns or rows_

#### `<col>`
Attribute|Description
-:|-
span|_Specifies the number of columns to span_

#### `<colgroup>`
Attribute|Description
-:|-
span|_Specifies the number of columns to span_

### VISIBLE ELEMENTS' ATTRIBUTES
> [<<<](#)

**These attributes can be used with all visible HTML elements.**
Attribute|Description
-:|-
onblur|_Script to be run when the element loses focus_
onchange|_Script to be run when the value of the element is changed_
onclick|_Script to be run when the element is being clicked_
oncontextmenu|_Script to be run when a context menu is triggered_
oncopy|_Script to be run when the content of the element is being copied_
oncut|_Script to be run when the content of the element is being cut_
ondblclick|_Script to be run when the element is being double-clicked_
ondrag|_Script to be run when the element is being dragged_
ondragend|_Script to be run at the end of a drag operation_
ondragenter|_Script to be run when an element has been dragged to a valid drop target_
ondragleave|_Script to be run when an element leaves a valid drop target_
ondragover|_Script to be run when an element is being dragged over a valid drop target_
ondragstart|_Script to be run at the start of a drag operation_
ondrop|_Script to be run when dragged element is being dropped_
onfocus|_Script to be run when the element gets focus_
oninput|_Script to be run when the element gets user input_
oninvalid|_Script to be run when the element is invalid_
onkeydown|_Script to be run when a user is pressing a key_
onkeypress|_Script to be run when a user presses a key_
onkeyup|_Script to be run when a user releases a key_
onmousedown|_Script to be run when a mouse button is pressed down on an element_
onmousemove|_Script to be run as long as the  mouse pointer is moving over an element_
onmouseout|_Script to be run when a mouse pointer moves out of an element_
onmouseover|_Script to be run when a mouse pointer moves over an element_
onmouseup|_Script to be run when a mouse button is released over an element_
onmousewheel|_Script to be run when a mouse wheel is being scrolled over an element_
onpaste|_Script to be run when the user pastes some content in an element_
onscroll|_Script to be run when an element's scrollbar is being scrolled_
onselect|_Script to be run when the element gets selected_
onwheel|_Script to be run when the mouse wheel rolls up or down over an element_

### WIDGET ATTRIBUTES
> [<<<](#)
#### `<details>`
Attribute|Description
-:|-
ontoggle|_Script to be run when the user opens or closes the \<details> element_
open|_Specifies that the details should be visible (open) to the user_

## -
[<<<](#)
~~~
<!--...-->	Insert comment into the source code
  <!--This is a comment. Comments are not displayed in the browser-->
  <!--This comment prevents run a JavaScript code-->
    <script type="text/javascript">
    <!--
      function displayMsg() {
        alert("Hello World!")
      }
    //-->
    </script> 
<!DOCTYPE> 	Defines the document type
  <!--This is an information to the browser about HTML5 document--> 
    <!DOCTYPE html>
  <!--This is an information to the browser about HTML4 document--> 
    <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
  <!--This is an information to the browser about XHTML document--> 
    <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
~~~

## A
[<<<](#)
~~~
<a>		Defines a hyperlink
  <!-- Reference to a hyperlink>
    <a href="https://www.w3schools.com">Visit W3Schools.com!</a>

<abbr>		Defines an abbreviation or an acronym
<acronym>	Not supported in HTML5. Use <abbr> instead. Defines an acronym
<address>	Defines contact information for the author/owner of a document
<applet>	Not supported in HTML5. Use <embed> or <object> instead. Defines an embedded applet
<area>		Defines an area inside an image map
<article>	Defines an article
<aside>		Defines content aside from the page content
<audio>		Defines embedded sound content

accept		Specifies the types of files that the server accepts (only for type="file")
accept-charset	Specifies the character encodings that are to be used for the form submission
accesskey	Specifies a shortcut key to activate/focus an element
action		Specifies where to send the form-data when a form is submitted
align		Not supported in HTML 5. Specifies the alignment according to surrounding elements. Use CSS instead
alt		Specifies an alternate text when the original element fails to display
async		Specifies that the script is executed asynchronously (only for external scripts)
autocomplete	Specifies whether the <form> or the <input> element should have autocomplete enabled
autofocus	Specifies that the element should automatically get focus when the page loads
autoplay	Specifies that the audio/video will start playing as soon as it is ready
~~~

## B
[<<<](#)
~~~
<b>		Defines bold text
<base>		Specifies the base URL/target for all relative URLs in a document
<basefont>	Not supported in HTML5. Use CSS instead. Specifies a default color, size, and font for all text in a document
<bdi>		Isolates a part of text that might be formatted in a different direction from other text outside it
<bdo>		Overrides the current text direction
<big>		Not supported in HTML5. Use CSS instead. Defines big text
<blockquote>	Defines a section that is quoted from another source
<body>		Defines the document's body
<br>		Defines a single line break
<button>	Defines a clickable button

bgcolor		Not supported in HTML 5. Specifies the background color of an element. Use CSS instead
border		Not supported in HTML 5. Specifies the width of the border of an element. Use CSS instead
~~~

## C
[<<<](#)
~~~
<canvas>	Used to draw graphics, on the fly, via scripting (usually JavaScript)
<caption>	Defines a table caption
<center>	Not supported in HTML5. Use CSS instead. Defines centered text
<cite>		Defines the title of a work
<code>		Defines a piece of computer code
<col>		Specifies column properties for each column within a <colgroup> element 
<colgroup>	Specifies a group of one or more columns in a table for formatting

charset		Specifies the character encoding
checked		Specifies that an <input> element should be pre-selected when the page loads (for type="checkbox" or type="radio")
cite		Specifies a URL which explains the quote/deleted/inserted text
class		Specifies one or more classnames for an element (refers to a class in a style sheet)
color		Not supported in HTML 5. Specifies the text color of an element. Use CSS instead
cols		Specifies the visible width of a text area
colspan		Specifies the number of columns a table cell should span
content		Gives the value associated with the http-equiv or name attribute
contenteditable	Specifies whether the content of an element is editable or not
controls	Specifies that audio/video controls should be displayed (such as a play/pause button etc)
coords		Specifies the coordinates of the area
~~~

## D
[<<<](#)
~~~
<data>		Adds a machine-readable translation of a given content
<datalist>	Specifies a list of pre-defined options for input controls
<dd>		Defines a description/value of a term in a description list
<del>		Defines text that has been deleted from a document
<details>	Defines additional details that the user can view or hide
<dfn>		Specifies a term that is going to be defined within the content
<dialog>	Defines a dialog box or window
<dir>		Not supported in HTML5. Use <ul> instead. Defines a directory list
<div>		Defines a section in a document
<dl>		Defines a description list
<dt>		Defines a term/name in a description list

data		Specifies the URL of the resource to be used by the object
data-*		Used to store custom data private to the page or application
datetime	Specifies the date and time
default		Specifies that the track is to be enabled if the user's preferences do not indicate that another track would be more appropriate
defer		Specifies that the script is executed when the page has finished parsing (only for external scripts)
dir		Specifies the text direction for the content in an element
dirname		Specifies that the text direction will be submitted
disabled	Specifies that the specified element/group of elements should be disabled
download	Specifies that the target will be downloaded when a user clicks on the hyperlink
draggable	Specifies whether an element is draggable or not
~~~

## E

[<<<](#)
~~~
<em>		Defines emphasized text 
<embed>		Defines a container for an external application

enctype		Specifies how the form-data should be encoded when submitting it to the server (only for method="post")
~~~

## F

[<<<](#)
~~~
<fieldset>	Groups related elements in a form
<figcaption>	Defines a caption for a <figure> element
<figure>	Specifies self-contained content
<font>		Not supported in HTML5. Use CSS instead. Defines font, color, and size for text
<footer>	Defines a footer for a document or section
<form>		Defines an HTML form for user input
<frame>		Not supported in HTML5. Defines a window (a frame) in a frameset
<frameset>	Not supported in HTML5. Defines a set of frames

for		Specifies which form element(s) a label/calculation is bound to
form		Specifies the name of the form the element belongs to
formaction	Specifies where to send the form-data when a form is submitted. Only for type="submit"
~~~

## G

[<<<](#)
~~~
~~~

## H

[<<<](#)
~~~
<h1>…<h6>	Defines HTML headings
<head>		Contains metadata/information for the document
<header>	Defines a header for a document or section
<hr>		Defines a thematic change in the content
<html>		Defines the root of an HTML document

headers		Specifies one or more headers cells a cell is related to
height		Specifies the height of the element
hidden		Specifies that an element is not yet, or is no longer, relevant
high		Specifies the range that is considered to be a high value
href		Specifies the URL of the page the link goes to
	href="": Placeholder for a hyperlink
hreflang	Specifies the language of the linked document
http-equiv	Provides an HTTP header for the information/value of the content attribute
~~~

## I

[<<<](#)
~~~
<i>		Defines a part of text in an alternate voice or mood
<iframe>	Defines an inline frame
<img>		Defines an image
<input>		Defines an input control
<ins>		Defines a text that has been inserted into a document

id		Specifies a unique id for an element
ismap		Specifies an image as a server-side image map
~~~

## J

[<<<](#)
~~~
~~~

## K

[<<<](#)
~~~
<kbd>		Defines keyboard input
<keygen>	Encryption

kind		Specifies the kind of text track
~~~

## L

[<<<](#)
~~~
<label>		Defines a label for an <input> element
<legend>	Defines a caption for a <fieldset> element
~~~
>[\<li>](./README.md#list) Defines a list item
~~~
<link>		Defines the relationship between a document and an external resource (most used to link to style sheets)

label		Specifies the title of the text track
lang		Specifies the language of the element's content
list		Refers to a <datalist> element that contains pre-defined options for an <input> element
loop		Specifies that the audio/video will start over again, every time it is finished
low		Specifies the range that is considered to be a low value
~~~

## M

[<<<](#)
~~~
<main>		Specifies the main content of a document
<map>		Defines an image map
<mark>		Defines marked/highlighted text
<meta>		Defines metadata about an HTML document
<meter>		Defines a scalar measurement within a known range (a gauge)

max		Specifies the maximum value
maxlength	Specifies the maximum number of characters allowed in an element
media		Specifies what media/device the linked document is optimized for
method		Specifies the HTTP method to use when sending form-data
min		Specifies a minimum value
multiple	Specifies that a user can enter more than one value
muted		Specifies that the audio output of the video should be muted
~~~

## N

[<<<](#)
~~~
<nav>		Defines navigation links
<noframes>	Not supported in HTML5. Defines an alternate content for users that do not support frames
<noscript>	Defines an alternate content for users that do not support client-side scripts

name		Specifies the name of the element
novalidate	Specifies that the form should not be validated when submitted
~~~

## O

[<<<](#)
~~~
<object>	Defines a container for an external application
<ol>		Defines an ordered list
<optgroup>	Defines a group of related options in a drop-down list
<option>	Defines an option in a drop-down list
<output>	Defines the result of a calculation

onabort		Script to be run on abort
onafterprint	Script to be run after the document is printed
onbeforeprint	Script to be run before the document is printed
onbeforeunload	Script to be run when the document is about to be unloaded
onblur		Script to be run when the element loses focus
oncanplay	Script to be run when a file is ready to start playing (when it has buffered enough to begin)
oncanplaythroughScript to be run when a file can be played all the way to the end without pausing for buffering
onchange	Script to be run when the value of the element is changed
onclick		Script to be run when the element is being clicked
oncontextmenu	Script to be run when a context menu is triggered
oncopy		Script to be run when the content of the element is being copied
oncuechange	Script to be run when the cue changes in a <track> element
oncut		Script to be run when the content of the element is being cut
ondblclick	Script to be run when the element is being double-clicked
ondrag		Script to be run when the element is being dragged
ondragend	Script to be run at the end of a drag operation
ondragenter	Script to be run when an element has been dragged to a valid drop target
ondragleave	Script to be run when an element leaves a valid drop target
ondragover	Script to be run when an element is being dragged over a valid drop target
ondragstart	Script to be run at the start of a drag operation
ondrop		Script to be run when dragged element is being dropped
ondurationchangeScript to be run when the length of the media changes
onemptied	Script to be run when something bad happens and the file is suddenly unavailable (like unexpectedly disconnects)
onended		Script to be run when the media has reach the end (a useful event for messages like "thanks for listening")
onerror		Script to be run when an error occurs
onfocus		Script to be run when the element gets focus
onhashchange	Script to be run when there has been changes to the anchor part of the a URL
oninput		Script to be run when the element gets user input
oninvalid	Script to be run when the element is invalid
onkeydown	Script to be run when a user is pressing a key
onkeypress	Script to be run when a user presses a key
onkeyup		Script to be run when a user releases a key
onload		Script to be run when the element is finished loading
onloadeddata	Script to be run when media data is loaded
onloadedmetadataScript to be run when meta data (like dimensions and duration) are loaded
onloadstart	Script to be run just as the file begins to load before anything is actually loaded
onmousedown	Script to be run when a mouse button is pressed down on an element
onmousemove	Script to be run as long as the  mouse pointer is moving over an element
onmouseout	Script to be run when a mouse pointer moves out of an element
onmouseover	Script to be run when a mouse pointer moves over an element
onmouseup	Script to be run when a mouse button is released over an element
onmousewheel	Script to be run when a mouse wheel is being scrolled over an element
onoffline	Script to be run when the browser starts to work offline
ononline	Script to be run when the browser starts to work online
onpagehide	Script to be run when a user navigates away from a page
onpageshow	Script to be run when a user navigates to a page
onpaste		Script to be run when the user pastes some content in an element
onpause		Script to be run when the media is paused either by the user or programmatically
onplay		Script to be run when the media has started playing
onplaying	Script to be run when the media has started playing
onpopstate	Script to be run when the window's history changes.
onprogress	Script to be run when the browser is in the process of getting the media data
onratechange	Script to be run each time the playback rate changes (like when a user switches to a slow motion or fast forward mode).
onreset		Script to be run when a reset button in a form is clicked.
onresize	Script to be run when the browser window is being resized.
onscroll	Script to be run when an element's scrollbar is being scrolled
onsearch	Script to be run when the user writes something in a search field (for <input type="search">)
onseeked	Script to be run when the seeking attribute is set to false indicating that seeking has ended
onseeking	Script to be run when the seeking attribute is set to true indicating that seeking is active
onselect	Script to be run when the element gets selected
onstalled	Script to be run when the browser is unable to fetch the media data for whatever reason
onstorage	Script to be run when a Web Storage area is updated
onsubmit	Script to be run when a form is submitted
onsuspend	Script to be run when fetching the media data is stopped before it is completely loaded for whatever reason
ontimeupdate	Script to be run when the playing position has changed (like when the user fast forwards to a different point in the media)
ontoggle	Script to be run when the user opens or closes the <details> element
onunload	Script to be run when a page has unloaded (or the browser window has been closed)
onvolumechange	Script to be run each time the volume of a video/audio has been changed
onwaiting	Script to be run when the media has paused but is expected to resume (like when the media pauses to buffer more data)
onwheel		Script to be run when the mouse wheel rolls up or down over an element
open		Specifies that the details should be visible (open) to the user
optimum		Specifies what value is the optimal value for the gauge
~~~

## P

[<<<](#)
~~~
<p>		Defines a paragraph
<param>		Defines a parameter for an object
<picture>	Defines a container for multiple image resources
<pre>		Defines preformatted text
<progress>	Represents the progress of a task

pattern		Specifies a regular expression that an <input> element's value is checked against
placeholder	Specifies a short hint that describes the expected value of the element
poster		Specifies an image to be shown while the video is downloading, or until the user hits the play button
preload		Specifies if and how the author thinks the audio/video should be loaded when the page loads
~~~

## Q

[<<<](#)
~~~
<q>		Defines a short quotation
~~~

## R

[<<<](#)
~~~
<rp>		Defines what to show in browsers that do not support ruby annotations
<rt>		Defines an explanation/pronunciation of characters (for East Asian typography)
<ruby>		Defines a ruby annotation (for East Asian typography)

readonly	Specifies that the element is read-only
rel		Specifies the relationship between the current document and the linked document
required	Specifies that the element must be filled out before submitting the form
reversed	Specifies that the list order should be descending (9,8,7...)
rows		Specifies the visible number of lines in a text area
rowspan		Specifies the number of rows a table cell should span
~~~

## S

[<<<](#)
~~~
<s>		Defines text that is no longer correct
<samp>		Defines sample output from a computer program
<script>	Defines a client-side script
<section>	Defines a section in a document
<select>	Defines a drop-down list
<small>		Defines smaller text
<source>	Defines multiple media resources for media elements (<video> and <audio>)
<span>		Defines a section in a document
<strike>	Not supported in HTML5. Use <del> or <s> instead. Defines strikethrough text
<strong>	Defines important text
<style>		Defines style information for a document
<sub>		Defines subscripted text
<summary>	Defines a visible heading for a <details> element
<sup>		Defines superscripted text
<svg>		Defines a container for SVG graphics

sandbox		Enables an extra set of restrictions for the content in an <iframe>
scope		Specifies whether a header cell is a header for a column, row, or group of columns or rows
selected	Specifies that an option should be pre-selected when the page loads
shape		Specifies the shape of the area
size		Specifies the width, in characters (for <input>) or specifies the number of visible options (for <select>)
sizes		Specifies the size of the linked resource
span		Specifies the number of columns to span
spellcheck	Specifies whether the element is to have its spelling and grammar checked or not
src		Specifies the URL of the media file
srcdoc		Specifies the HTML content of the page to show in the <iframe>
srclang		Specifies the language of the track text data (required if kind="subtitles")
srcset		Specifies the URL of the image to use in different situations
start		Specifies the start value of an ordered list
step		Specifies the legal number intervals for an input field
style		Specifies an inline CSS style for an element
~~~

## T

[<<<](#)
~~~
<table>		Defines a table
<tbody>		Groups the body content in a table
<td>		Defines a cell in a table
<template>	Defines a container for content that should be hidden when the page loads
<textarea>	Defines a multiline input control (text area)
<tfoot>		Groups the footer content in a table
<th>		Defines a header cell in a table
<thead>		Groups the header content in a table
<time>		Defines a specific time (or datetime)
<title>		Defines a title for the document
<tr>		Defines a row in a table
<track>		Defines text tracks for media elements (<video> and <audio>)
<tt>		Not supported in HTML5. Use CSS instead. Defines teletype text

tabindex	Specifies the tabbing order of an element
target		Specifies the target for where to open the linked document or where to submit the form
title		Specifies extra information about an element
translate	Specifies whether the content of an element should be translated or not
type		Specifies the type of element
~~~

## U

[<<<](#)
~~~
<u>		Defines some text that is unarticulated and styled differently from normal text
<ul>		Defines an unordered list

usemap		Specifies an image as a client-side image map
~~~

## V

[<<<](#)
~~~
<var>		Defines a variable
<video>		Defines embedded video content

value		Specifies the value of the element
~~~

## W

[<<<](#)
~~~
<wbr>		Defines a possible line-break

width		Specifies the width of the element
wrap		Specifies how the text in a text area is to be wrapped when submitted in a form
~~~

## X

[<<<](#)
~~~
~~~

## Y

[<<<](#)
~~~
~~~

## Z

[<<<](#)
~~~


