<h1 align="center"><abbr title="Hypertext Markup Language"><img src="./img/html5_logo.webp"></abbr></h1>

> [![](./img/abc.webp)>>> index.md](index.md)

[Elements:](#elements)
- [Tags](#tags)
- [Attributes](#attributes)
  - [Names](#names)
  - [Values](#values)
- [Contents](#contents)

## Elements
[<<< HTML5](#)
> [<abbr title="Document Object Model">HTML DOM Elements</abbr>](#html-dom-elements)

Element|Description
-:|-   
`<tag>`|_self-enclosing element_
`<tag attribute="value">`|_self-enclosing element with attribute and value_
`<tag attribute="value" attribute="value" …>`|_self-enclosing element with attributes and values_
`<tag>Content</tag>`|_element with content_
`<tag attribute="value">Content</tag>`|_element with attribute, value and content_
`<tag attribute="value" attribute="value" …>Content</tag>`|_element with attributes, values and content_

---

## Tags
[<<< HTML5](#)
Tag|Description
-|-
[Comment](#comment)|_Defines the document type or insert comment into the source code_
[Structure](#structure)|_Defines the structure of an HTML document_
[Metadata](#metadata)|_Defines metadata/information for the document between `<head>…</head>` tags_
[Container](#container)|_Defines a container for other element(s)_
[Separator](#separator)|
[Text](#text)|
[List](#list)|
[Table](#table)|
[Form](#form)|
[Link](#link)|
[Media](#media)|
[JavaScript](#javascript)|
[Not supported](#not-supported)|

---

### Comment
[<<< Tags](#tags)
- Defines the document type or insert comment into the source code

HTML Tag|Function
-|-
[`<!DOCTYPE>`](#doctype)|_Defines the document type_
[`<!-- … -->`](#------)|_Insert comment into the source code_

---

### Structure
[<<< Tags](#tags)
- Defines the structure of an HTML document

HTML Tag|Function
-|-
[`<html>…</html>`](#htmlhtml)|_Defines the root of an HTML document_
[`<head>…</head>`](#headhead)|_Contains metadata/information for the document_
[`<body>…</body>`](#bodybody)|_Defines the document's body_

- `<address>` Defines contact information for the author/owner of a document
- `<aside>` Defines content aside from the page content
- `<div>` Defines a section in a document
- `<footer>` Defines a footer for a document or section
- `<header>` Defines a header for a document or section
- `<main>` Specifies the main content of a document
- `<section>` Defines a block section in a document

**Structure example:**
~~~
  <!DOCTYPE html>
  <html>
    <head>
      <meta …>
      <base …>
      <link …>
      <title>…</title>
    </head>
    <body>
      <header>
        <nav>
          <a href="…">…</a>
        </nav>
      </header>
      <main>
        <section>
          <div>
            <article>…</article> 
          </div>
        </section>
        <aside>
        </aside> 
      </main>
      <footer>
        <address>…</address> 
        <noscript>…</noscript>
        <script>…</script>
      </footer>
    </body>
  </html>
~~~

**index.html example**:
```
  <!DOCTYPE html>
  <html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document title</title>
  </head>
  <body>
    Hello World!
  </body>
  </html>
```

---

### Metadata
[<<< Tags](#tags)
- Defines metadata/information for the document between `<head>…</head>` tags

HTML Tag|Function
-:|-
[`<meta …>`](#meta)|_Defines metadata about an HTML document_
[`<title>…</title>`](#titletitle)|_Defines a title for the document_
[`<base …>`](#base)|_Specifies the base URL/target for all relative URLs in a document_
[`<link …>`](#link)|_Defines the relationship between a document and an external resource_
[`<style>…</style>`](#stylestyle)|_Defines style information for a document_

- `<base>` Specifies the base URL/target for all relative URLs in a document
- `<link>` Defines the relationship between a document and an external resource (most used to link to style sheets)
- `<meta>` Defines metadata about an HTML document
- `<style>` Defines metadata about an HTML document (Use <link …> to external style sheet instead.)
- `<title>` Defines a title for the document

---

### Container
[<<< Tags](#tags)
- Defines a container for other element(s)
  - `<data>` Adds a machine-readable translation of a given content
  - `<details>` Defines additional details that the user can view or hide
  - `<embed>` Defines a container for an external application
  - `<iframe>` Defines an inline frame
  - `<object>` Defines a container for an external application
  - `<p>` Defines a paragraph
  - `<param>` Defines a parameter for an object
  - `<span>` Defines an inline section in a document
  - `<summary>` Defines a visible heading for a \<details> element
  - `<svg>` Defines a container for SVG graphics

---

### Separator
[<<< Tags](#tags)
- [`<br>`](#br) Defines a single line break
- [`<hr>`](#hr) Defines a thematic change in the content
- [`<wbr>`](#wbr) Defines a possible line-break

---

### Text
> [<<< Tags](#tags)

Type|Description
-|-
[Code](#code)|_Defines a program or keyboard code_
[Direction](#direction)|_Defines text direction_
[Format](#format)|_Text formatting_
[Kind](#kind)|_Defines a kind of text_
[Quote](#quote)|_Defines a quote_
[Ruby](#ruby)|_Defines a ruby annotation_

#### Code
> [<<< Text](#text)
- Defines a program or keyboard code
  - `<code>` Defines a piece of computer code
  - [`<kbd>…</kbd>`](#kbdkbd) Defines keyboard input
  - `<samp>` Defines sample output from a computer program 
  - `<var>` Defines a variable

#### Direction
> [<<< Text](#text)
- Defines text direction
  - `<bdi>` Isolates a part of text that might be formatted in a different direction from other text outside it
  - `<bdo>` Overrides the current text direction

#### Format
> [<<< Text](#text)
- Text formatting

Tag|Decription
-:|-
[`<b>…</b>`](#bb)|_Defines bold text_
[`<del>…</del>`](#deldel)|_Defines text that has been deleted from a document_
[`<em>…</em>`](#emem)|_Defines emphasized text_
[`<h1>…</h1>-<h6>…</h6>`](#h1h1--h6h6)|_Defines HTML heading_
[`<i>…</i>`](#ii)|_Defines a part of text in an italic style (alternate voice or mood)_
[`<ins>…</ins>`](#insins)|_Defines a text that has been inserted into a document_
[`<mark>…</mark>`](#markmark)|_Defines marked/highlighted text_
[`<s>…</s>`](#ss)|_Defines text with strikethrough (that is no longer correct)_
[`<small…</small>`](#smallsmall)|_Defines small(er) text_
[`<strong>…</strong>`](#strongstrong)|_Defines strong (important) text_
[`<sub>…</sub>`](#subsub)|_Defines subscripted text_
[`<sup>…</sup>`](#supsup)|_Defines superscripted text_
[`<u>…</u>`](#uu)|_Defines underlined text (that is articulated and styled differently from normal text)_

#### Kind
> [<<< Text](#text)
- Defines a kind of text
[`<abbr>…</abbr>`](#abbrabbr) Defines an abbreviation or an acronym
  - `<article>` Defines an article
  - `<cite>` Defines the title of a work
  - `<dfn>` Specifies a term that is going to be defined within the content
  - [`<pre>`](#prepre) Defines preformatted text
  - `<time>` Defines a specific time (or datetime)

#### Quote
> [<<< Text](#text)
- Defines a quote
  - `<blockquote>` Defines a section that is quoted from another source
  - `<q>` Defines a short quotation

#### Ruby
> [<<< Text](#text)
- Defines a ruby annotation
  - `<rp>` Defines what to show in browsers that do not support ruby annotations
  - `<rt>` Defines an explanation/pronunciation of characters (for East Asian typography)
  - `<ruby>` Defines a ruby annotation (for East Asian typography)

---

### List
[<<< Tags](#tags)
> [Ordered list](#ordered-list)
> [Unordered list](#unordered-list)
> [Description list](#description-list)

#### Ordered list
[<<< List](#list)
- `<ol>` Defines an ordered list
  - There are 4 types with attribute name **type** of ordered list:
    - `type="1"` This creates a numbered list starting from `1` (default).
    - `type="A"` This creates a list numbered with uppercase letters starting from `A`.
    - `type="a"` This creates a list numbered with lowercase letters starting from `a`.
    - `type="I"` This creates a list numbered with uppercase roman numbers starting from `I`.
    - `type="i"` This creates a list numbered with lowercase roman numbers starting from `i`.
    - Another starting numbers/characters are available with attribute name **start** (e.g. `start="5"`).
- `<li>` Defines a list item

_Code:_
~~~
<ol>
  <li>list item</li>
  <li>another list item</li>
</ol>
~~~
_Result:_
<ol>
  <li>list item</li>
  <li>another list item</li>
</ol>

#### Unordered list
[<<< List](#list)
- `<ul>` Defines an unordered list
  - There are 4 types with attribute name **style** of unordered list:
    - `style="list-style-type:disc"` Creates an unordered list marked to a bullet (default).
    - `style="list-style-type:circle"` Creates an unordered list marked to a circle.
    - `style="list-style-type:square"` Creates an unordered list marked to a square.
    - `style="list-style-type:none"` Creates an unordered list without any marker.
- `<li>` Defines a list item

_Code:_
~~~
  <ul>
    <li>list item</li>
      <ul>
        <li>list subitem</li>
          <ul>
            <li>list sub-subitem</li>
          </ul>
      </ul>
    <li>another list item</li>
  </ol>
~~~  
_Result:_
  <ul>
    <li>list item</li>
      <ul>
        <li>list subitem</li>
          <ul>
            <li>list sub-subitem</li>
          </ul>
      </ul>
    <li>another list item</li>
  </ul>

#### Description list
[<<< List](#list)
- `<dl>` Defines a description list
- `<dt>` Defines a term/name in a description list
- `<dd>` Description details: defines a description/value of a term in a description list

_Code:_
~~~
  <dl>
    <dt>Description name
      <dd>value1</dd> 
      <dd>value2</dd> 
    </dt>
    <dt>Another description name
      <dd>another value</dd> 
    </dt>
  </dl>
~~~
_Result:_
  <dl>
    <dt>Description name
      <dd>value1</dd> 
      <dd>value2</dd> 
    </dt>
    <dt>Another description name
      <dd>another value</dd> 
    </dt>
  </dl>

---

### Table
[<<< Tags](#tags)
- `<table>` Defines a table
  - `<caption>` Defines a table caption
  - `<colgroup>` Specifies a group of one or more columns in a table for formatting
    - `<col>` Specifies column properties for each column within a <colgroup> element 
  - `<thead>` Groups the header content in a table
    - `<tr>` Defines a row in a table
      - `<th>` Defines a header cell in a table
  - `<tbody>` Groups the body content in a table
    - `<tr>` Defines a row in a table
      - `<td>` Defines a cell in a table
  - `<tfoot>` Groups the footer content in a table
    - `<tr>` Defines a row in a table
      - `<td>` Defines a cell in a table

_Code:_
~~~
  <table>
    <caption>Table caption</caption>
    <thead>
      <tr>
        <th>header1</th>
        <th>header2</th>
        <th>header3</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>normal data</td>
        <td>data1</td>
        <td>data2</td>
      </tr>
      <tr>
        <td rowspan="2">data with rowspan</td>
        <td>data3</td>
        <td>data4</td>
      </tr>
      <tr>
        <td>data5</td>
        <td>data6</td>
      </tr>
    </tbody>
    <tfoot>
      <tr>
        <td>foot data</td>
        <td colspan="2">foot data with colspan</td>
      </tr>
    </tfoot>
  </table>
~~~
_Result:_
  <table>
    <caption>Table caption</caption>
    <thead>
      <tr>
        <th>header1</th>
        <th>header2</th>
        <th>header3</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>normal data</td>
        <td>data1</td>
        <td>data2</td>
      </tr>
      <tr>
        <td rowspan="2">data with rowspan</td>
        <td>data3</td>
        <td>data4</td>
      </tr>
      <tr>
        <td>data5</td>
        <td>data6</td>
      </tr>
    </tbody>
    <tfoot>
      <tr>
        <td>foot data</td>
        <td colspan="2">foot data with colspan</td>
      </tr>
    </tfoot>
  </table>

---

### Form
[<<< Tags](#tags)
- `<button>` Defines a clickable button
- `<datalist>` Specifies a list of pre-defined options for input controls
- `<dialog>` Defines a dialog box or window
- `<fieldset>` Groups related elements in a form
- `<form>` Defines an HTML form for user input
- `<input>` Defines an input control
- `<label>` Defines a label for an \<input> element
- `<legend>` Defines a caption for a \<fieldset> element
- `<meter>` Defines a scalar measurement within a known range (a gauge)
- `<optgroup>` Defines a group of related options in a drop-down list
- `<option>` Defines an option in a drop-down list
- `<output>` Defines the result of a calculation
- `<progress>` Represents the progress of a task
- `<select>` Defines a drop-down list
- `<textarea>` Defines a multiline input control (text area)

---

### Link
[<<< Tags](#tags)

HTML Tag|Function
-|:-:
[\<a>…\</a>](#aa)|defines a hyperlink

- `<a>` Defines a hyperlink
- `<nav>` Defines navigation links
 
---

### Media
> [<<< { Tags }](#tags)
> [>>> { Image }](#image)
> [>>> { Graphics }](#graphics)
> [>>> { Audio & Video }](#audio--video)

#### Image
- `<area>` Defines an area inside an image map
- [`<img>`](#imgimg) Defines an image
- `<map>` Defines an image map
- `<picture>` Defines a container for multiple image resources

#### Graphics
[<<< Tags](#tags)
- `<canvas>` Used to draw graphics, on the fly, via scripting (usually JavaScript)
- `<figcaption>` Defines a caption for a \<figure> element
- `<figure>` Specifies self-contained content

#### Audio & Video
- `<audio>` Defines embedded sound content
- `<source>` Defines multiple media resources for media elements (\<video> and \<audio>)
- `<track>` Defines text tracks for media elements (\<video> and \<audio>)
- `<video>` Defines embedded video content

---

### JavaScript
[<<< Tags](#tags)
- `<noscript>` Defines an alternate content for users that do not support client-side scripts
- `<script>` Defines a client-side script
- `<template>` Defines a container for content that should be hidden when the page loads

### Not supported
[<<< Tags](#tags)

- `<acronym>` Not supported in HTML5. Use \<abbr> instead. Defines an acronym
- `<applet>` Not supported in HTML5. Use \<embed> or \<object> instead. Defines an embedded applet
- `<basefont>` Not supported in HTML5. Use CSS instead. Specifies a default color, size, and font for all text in a document
- `<big>` Not supported in HTML5. Use CSS instead. Defines big text
- `<center>` Not supported in HTML5. Use CSS instead. Defines centered text
- `<dir>` Not supported in HTML5. Use \<ul> instead. Defines a directory list
- `<font>` Not supported in HTML5. Use CSS instead. Defines font, color, and size for text
- `<frame>` Not supported in HTML5. Defines a window (a frame) in a frameset
- `<frameset>` Not supported in HTML5. Defines a set of frames
- `<menu>` Not supported in most browsers (Firefox support only). Use \<ul> instead
- `<menuitem>` Not supported in most browsers (Firefox support only). Use \<ul> instead
- `<noframes>` Not supported in HTML5. Defines an alternate content for users that do not support frames
- `<strike>` Not supported in HTML5. Use \<del> or \<s> instead. Defines strikethrough text
- `<tt>` Not supported in HTML5. Use CSS instead. Defines teletype text

---

## Attributes

[<<< HTML5 index](#)
- [Global attributes](#global-attributes)
- [Event attributes](#event-attributes)
- [Not supported attributes](#not-supported-attributes)
  
---

### Global attributes

[<<< Attributes](#attributes)
- Global attributes can be used on all elements (though they may have no effect on some elements).

attribute|_description_
-:|-
`accesskey`|_Specifies a shortcut key to activate/focus an element_
`class`|_Specifies one or more classnames for an element (refers to a class in a style sheet)_
`contenteditable`|Specifies whether the content of an element is editable or not_
`data-*`|_Used to store custom data private to the page or application_
`dir`|_Specifies the text direction for the content in an element_
`draggable`|_Specifies whether an element is draggable or not_
`hidden`|_Specifies that an element is not yet, or is no longer, relevant_
`id`|_Specifies a unique id for an element_
`lang`|_Specifies the language of the element's content_
`spellcheck`|_Specifies whether the element is to have its spelling and grammar checked or not_
`style`|_Specifies an inline CSS style for an element_
`tabindex`|_Specifies the tabbing order of an element_
`title`|_Specifies extra information about an element_
`translate`|_Specifies whether the content of an element should be translated or not_

---

### Event attributes

[<<< Attributes](#attributes)
- HTML has the ability to let events trigger actions in a browser
- [Window event](#window-event)
- [Form event](#form-event)
- [Mouse event](#mouse-event)
- [Drag event](#drag-event)
- [Clipboard event](#clipboard-event)
- [Media event](#media-event)
- [\<detail> event](#detail-event)

---

#### Window event

[<<< Event attributes](#event-attributes)
- Events triggered for the window object (applies to the <body> tag)

attribute|_description_
-:|-
`onafterprint`|_Script to be run after the document is printed_
`onbeforeprint`|_Script to be run before the document is printed_
`onbeforeunload`|_Script to be run when the document is about to be unloaded_
`onerror`|_Script to be run when an error occurs_
`onhashchange`|_Script to be run when there has been changes to the anchor part of the a URL_
`onload`|_Fires after the page is finished loading_
`onmessage`|_Script to be run when the message is triggered_
`onoffline`|_Script to be run when the browser starts to work offline_
`ononline`|_Script to be run when the browser starts to work online_
`onpagehide`|_Script to be run when a user navigates away from a page_
`onpageshow`|_Script to be run when a user navigates to a page_
`onpopstate`|_Script to be run when the window's history changes_
`onresize`|_Fires when the browser window is resized_
`onstorage`|_Script to be run when a Web Storage area is updated_
`onunload`|_Fires once a page has unloaded (or the browser window has been closed)_

---

#### Form event

[<< Event attributes](#event-attributes)
- Events triggered by actions inside a HTML form (applies to almost all HTML elements, but is most used in form elements)

attribute|_description_
-:|-
`onblur`|_Fires the moment that the element loses focus_
`onchange`|_Fires the moment when the value of the element is changed_
`oncontextmenu`|_Script to be run when a context menu is triggered_
`onfocus`|_Fires the moment when the element gets focus_
`oninput`|_Script to be run when an element gets user input_
`oninvalid`|_Script to be run when an element is invalid_
`onreset`|_Fires when the Reset button in a form is clicked_
`onsearch`|_Fires when the user writes something in a search field (for \<input="search">)_
`onselect`|_Fires after some text has been selected in an element_
`onsubmit`|_Fires when a form is submitted_

---

#### Mouse event

[<<< Event attributes](#event-attributes)

attribute|_description_
-:|-
`onclick`|_Fires on a mouse click on the element_
`ondblclick`|_Fires on a mouse double-click on the element_
`onmousedown`|_Fires when a mouse button is pressed down on an element_
`onmousemove`|_Fires when the mouse pointer is moving while it is over an element_
`onmouseout`|_Fires when the mouse pointer moves out of an element_
`onmouseover`|_Fires when the mouse pointer moves over an element_
`onmouseup`|_Fires when a mouse button is released over an element_
`onmousewheel`|_Deprecated. Use the onwheel attribute instead_
`onwheel`|_Fires when the mouse wheel rolls up or down over an element _

---

#### Drag event

[<<< Event attributes](#event-attributes)

attribute|_description_
-:|-
`ondrag`|_Script to be run when an element is dragged_
`ondragend`|_Script to be run at the end of a drag operation_
`ondragenter`|_Script to be run when an element has been dragged to a valid drop target_
`ondragleave`|_Script to be run when an element leaves a valid drop target_
`ondragover`|_Script to be run when an element is being dragged over a valid drop target_
`ondragstart`|_Script to be run at the start of a drag operation_
`ondrop`|_Script to be run when dragged element is being dropped_
`onscroll`|_Script to be run when an element's scrollbar is being scrolled_

---

#### Clipboard event

[<<< Event attributes](#event-attributes)

attribute|_description_
-:|-
`oncopy`|_Fires when the user copies the content of an element_
`oncut`|_Fires when the user cuts the content of an element_
`onpaste`|_Fires when the user pastes some content in an element_

---

#### Media event

[<<< Event attributes](#event-attributes)
- Events triggered by medias like videos, images and audio (applies to all HTML elements, but is most common in media elements, like `<audio>`, `<embed>`, `<img>`, `<object>` and `<video>`).

attribute|_description_
-:|-
`onabort`|_Script to be run on abort_
`oncanplay`|_Script to be run when a file is ready to start playing (when it has buffered enough to begin)_
`oncanplaythrough`|_Script to be run when a file can be played all the way to the end without pausing for buffering_
`oncuechange`|_Script to be run when the cue changes in a <track> element_
`ondurationchange`|_Script to be run when the length of the media changes_
`onemptied`|_Script to be run when something bad happens and the file is suddenly unavailable (like unexpectedly disconnects)_
`onended`|_Script to be run when the media has reach the end (a useful event for messages like "thanks for listening")_
`onerror`|_Script to be run when an error occurs when the file is being loaded_
`onloadeddata`|_Script to be run when media data is loaded_
`onloadedmetadata`|_Script to be run when meta data (like dimensions and duration) are loaded_
`onloadstart`|_Script to be run just as the file begins to load before anything is actually loaded_
`onpause`|_Script to be run when the media is paused either by the user or programmatically_
`onplay`|_Script to be run when the media is ready to start playing_
`onplaying`|_Script to be run when the media actually has started playing_
`onprogress`|_Script to be run when the browser is in the process of getting the media data_
`onratechange`|_Script to be run each time the playback rate changes (like when a user switches to a slow motion or fast forward mode)_
`onseeked`|_Script to be run when the seeking attribute is set to false indicating that seeking has ended_
`onseeking`|_Script to be run when the seeking attribute is set to true indicating that seeking is active_
`onstalled`|_Script to be run when the browser is unable to fetch the media data for whatever reason_
`onsuspend`|_Script to be run when fetching the media data is stopped before it is completely loaded for whatever reason_
`ontimeupdate`|_Script to be run when the playing position has changed (like when the user fast forwards to a different point in the media)_
`onvolumechange`|_Script to be run each time the volume is changed which (includes setting the volume to "mute")_
`onwaiting`|_Script to be run when the media has paused but is expected to resume (like when the media pauses to buffer more data)_

---

#### \<detail> event

[<<< Event attributes](#event-attributes)

attribute|_description_
-:|-
`ontoggle`|_Fires when the user opens or closes the_ `<details>` _element_

---

### Not supported attributes

[<<< Attributes](#attributes)
attribute|_description_
-:|-
`align`|_Not supported in HTML 5. Specifies the alignment according to surrounding elements. Use CSS instead_
`bgcolor`|_Not supported in HTML 5. Specifies the background color of an element. Use CSS instead_
`border`|_Not supported in HTML 5. Specifies the width of the border of an element. Use CSS instead_
`color`|_Not supported in HTML 5. Specifies the text color of an element. Use CSS instead_

---

## HTML DOM Elements
[<<< HTML5](#)
- When a web page is loaded, the browser creates a Document Object Model of the page:
![HTML DOM tree of objects](./img/html_dom_tree_of_objects.gif)
- With the HTML DOM JavaScript can create dynamic HTML:
  - access and change all the elements of an HTML document
  - change all the HTML elements, attributes and CSS styles in the page
  - add new and remove existing HTML elements and attributes
  - react to all existing and create new HTML events in the page

---

### `<!-- … -->`

[<<< Comment tags](#comment-tags)
- Insert comment into the source code

HTML code| HTML view
-|-
`<!-- My first comment -->`|

---

### `<!DOCTYPE …>`

[<<< Comment tags](#comment-tags)
- Defines the document type

HTML code|View
-|-
`<!DOCTYPE html>`|

---

### `<a>…</a>`

[<< {Link}](#link)
- Defines a hyperlink
- Common atributes:
  - `<a href="…">`

HTML code|View
-|-
`<a href="#">Back to top</a>`|<a href="#">Back to top</a>
`<a href="#link">Back to section link</a>`|<a href="#link">Back to section link</a>
`<a href="./subfolder/page.md">Link to page.md file in a subfolder\</a>`|<a href="./subfolder/page.md">Link to page.md file in a subfolder</a>
`<a href="../README.md">Link to README.md file in parent folder\</a>`|<a href="../README.md">Link to README.md file in parent folder</a>
`<a href="https://www.google.com"></a>`|<a href="https://www.google.com">Link to web</a>
`<img src="sun.webp" alt="Link to an unreachable picture">`|<img src="sun.webp" alt="Link to an unreachable picture">
`<img src="./img/sun.jpg" alt="Link to a reachable picture">`|<img src="./img/sun.webp" alt="Link to a reachable picture" width="50">
`<a href="#">\<img src="./img/house%20icon.webp" alt="clickable picture"></a>`|<a href="#"><img src="./img/house%20icon.webp" alt="clickable picture" width="50"></a>
||Here is a simple footnote[^1].
[^1]: My reference.

---

### `<abbr>…</abbr>`
> [<<< { Text - Kind }](#kind)
- Defines an abbreviation or an acronym
- Inline elem
- Common atribute:
  - `<abbr title="…">` Text enclosed in quotes will be shown as a tooltip when the mouse pointer is over the abbreviation.

HTML code|View
-|-
`<abbr title="Hypertext Markup Language">HTML</abbr> is the standard markup language for creating Web pages.`|<abbr title="Hypertext Markup Language">HTML</abbr> is the standard markup language for creating Web pages.

---

### `<body>…</body>`

> [<<< { Structure }](#structure)
- document body

HTML code|View
-|-
`<body>`<br>`Hello World!`<br>`</body>`|Hello World!

---

### `<b>…</b>`
> [<<< { Text - Format }](#format)
- Defines bold text
- Inline elem

HTML code|View
-|-
`Text with <b>bold part</b> and normal part.`|Text with <b>bold part</b> and normal part.

---

### `<br>`
>[<<< { Tags - Separator }](#separator)
- Defines a single line break
- Sortörés (_break_) a szövegben (a szöveg folytatása a következő sorban jelenik meg)
- Blokk szintű elem

HTML code|View
-|-
`This is a text.`<br>`This is another text.`|This is a text.This is another text.
`This is a text.<br>`<br>`This is another text.`|This is a text.<br>This is another text.

---

### `<del>…</del>`
> [<<< { Text - Format }](#format)
- Defines text that has been deleted from a document
- Inline elem

HTML code|View
-|-
`Text with <del>deleted part</del> and normal part.`|Text with <del>deleted part</del> and normal part.

---

### `<em>…</em>`
> [<<< { Text - Format }](#format)
- Defines emphasized text
- Szövegrész kiemelése a többi szövegrésztől való megkülönböztetés céljából 
- Inline elem

HTML code|View
-|-
`Text with <em>emphasized part</em> and normal part.`|Text with <em>emphasized part</em> and normal part.

---

### `<h1>…</h1>`- `<h6>…</h6>`
> [<<< { Text - Format }](#format)
- Defines HTML heading
- Heading [_heding_] (fejléc) elemet hoz létre, ami arra való, hogy főcímet helyezzünk el az oldalunkon. 
- Blokk szintű elemek
- A `<h2>…</h2> - <h6>…</h6>`: szintén fejléc elemek, a növekvő számok egyre kisebb méretű alcímeket jelölnek.

HTML code|View
-|-
`<h1>Document title</h1>`|<h1>Document title</h1>|
`<h2>Document subtitle\</h2>`|<h2>Document subtitle</h2>
`<h3>Sub-subtitle\</h3>`|<h3>Sub-subtitle</h3>
`<h4>Sub-sub-subtitle\</h4>`|<h4>Sub-sub-subtitle</h4>
`<h5>Sub-sub-sub-subtitle\</h5>`|<h5>Sub-sub-sub-subtitle</h5>
`<h6>Sub-sub-sub-sub-subtitle\</h6>`|<h6>Sub-sub-sub-sub-subtitle</h6>

---

### `<head>…</head>`

[<< {Structure}](#structure)
- document head

HTML code|View
-|-
`<head>`<br>`…`<br>`</head>`|

---

### `<html>…</html>`

[<< {Structure}](#structure)
- HTML document
  - language: `lang="…"`

HTML code|View
-|-
`<html lang="en">`|
`<html lang="hu">`|

---

### `<hr>`
- Vízszintes vonal (horizontal rule) megjelenítése (pl. szövegrészek elkülönítésére)
- Blokk szintű elem

HTML code|View
-|-
`This is a text.<hr>This is another text.`|This is a text.<hr>This is another text.

---

### `<i>…</i>`
> [<<< { Text - Format }](#format)
- Defines a part of text in an italic style (alternate voice or mood)
- Inline elem

HTML code|View
-|-
`Text with <i>italic part</i> and normal part.`|Text with <i>italic part</i> and normal part.

---

### `<img>…</img>`
- Required attributes:
  - `src="…"`: _image source link_
  - `alt="…"`: _alternativ text (when image cannot reachable)_
- Common attributes:
  - `height="…"`: _image height_
  - `ismap`: _Specifies an image as a server-side image map. Allowed only if the `<img>` element is a descendant of an `<a>` element with a valid `href` attribute._
  - `loading="eager | lazy"`: _Specifies whether a browser should load an image immediately or to defer loading of images until some conditions are met_
  - `title="…"`: _image title (appearing text when mouse pointer is above)_
  - `width="…"`: _image width_

HTML code|View
-|-
`<img src="sun.webp" alt="Link to an unreachable picture">`|<img src="sun.webp" alt="Link to an unreachable picture">
`<img src="./img/sun.jpg" alt="Link to a reachable picture">`|<img src="./img/sun.webp" alt="Link to a reachable picture" width="50">

---

### `<ins>…</ins>`
> [<<< { Text - Format }](#format)
- Defines a text that has been inserted into a document
- Inline elem

HTML code|View
-|-
`Text with <ins>inserted part</ins> and normal part.`|Text with <ins>inserted part</ins> and normal part.

---

### `<kbd>…</kbd>`
> [<<< { Text - Code }](#code)
- Defines keyboard input
- Inline elem
- Most browsers will display this element with the following default CSS value:

```
kbd {
  font-family: monospace;
}
```

HTML code|View
-|-
`Press <kbd>CTRL + C</kbd> for copy selected text to clipboard.`|Press <kbd>CTRL + C</kbd> for copy selected text to clipboard.

---

### `<mark>…</mark>`
> [<<< { Text - Format }](#format)
- Defines marked/highlighted text
- Inline elem

HTML code|View
-|-
`Text with <mark>marked/highlighted part</mark> and normal part.`|Text with <mark>marked/highlighted part</mark> and normal part.

---

### `<meta …>`
[<< {Settings}](#settings)
- Supports global attributes

HTML code|View
-|-
`<meta charset="UTF-8">`|
`<meta http-equiv="X-UA-Compatible" content="IE=edge">`|
`<meta name="viewport" content="width=device-width, initial-scale=1.0">`|

---

### `<p>…</p>`
- Paragrafus: (paragraph [_peregref_]): a benne lévő szöveget új bekezdésben jeleníti meg (a kódban egymás után, új sorokba írt szövegek egyébként folyamatosan, sortörés nélkül jelennek meg
- Blokk szintű elem

HTML code|View
-|-
`This is not a paragraph.`<br>`This is not a paragraph.`|This is not a paragraph.This is not a paragraph.
`<p>This is a paragraph.</p>`<br>`<p>This is a paragraph.</p>`|<p>This is a paragraph.</p><p>This is a paragraph.</p>

---

### `<pre>…</pre>`
> [<<< { Text - Kind }](#kind)
- Defines preformatted text
- Kiemelt bekezdést hoz létre, megtartva azt a szövegformázást, amit a HTML kódban alkalmaztunk és egyforma szélességű karaktereket tartalmazó betűtípust használ.
- Blokk szintű elem

**HTML code:**
~~~
<pre>
 This is a preformatted text.
     This is a preformatted text.
</pre>
~~~
**HTML view:**
<pre>
 This is a preformatted text.
     This is a preformatted text.
</pre>

---

### `<s>…</s>`
> [<<< { Text - Format }](#format)
- Defines text with strikethrough (that is no longer correct)
- Inline elem

HTML code|View
-|-
`Text with <s>struck through part</s> and normal part.`|Text with <s>struck through part</s> and normal part.

---

### `<small>…</small>`
> [<<< { Text - Format }](#format)
- Defines small(er) text
- Inline elem

HTML code|View
-|-
`Text with <small>small(er) part</small> and normal part.`|Text with <small>small(er) part</small> and normal part.

---

### `<strong>…</strong>`
> [<<< { Text - Format }](#format)
- Defines strong (important) text
- Inline elem

HTML code|View
-|-
`Text with <strong>important part</strong> and normal part.`|Text with <strong>important part</strong> and normal part.

---

### `<sub>…</sub>`
> [<<< { Text - Format }](#format)
- Defines subscripted text
- Inline elem

HTML code|View
-|-
`Text with <sub>subscripted part</sub> and normal part.`|Text with <sub>subscripted part</sub> and normal part.

---

### `<sup>…</sup>`
> [<<< { Text - Format }](#format)
- Defines superscripted text
- Inline elem

HTML code|View
-|-
`Text with <sup>superscripted part</sup> and normal part.`|Text with <sup>superscripted part</sup> and normal part.

---

### `<title>…</title>`

[<< {Settings}](#settings)
- Document title displayed in the browser tab

HTML code|View
-|-

`<title>Document title</title>`

---

### `<u>…</u>`
> [<<< { Text - Format }](#format)
- Defines underlined text (that is articulated and styled differently from normal text)
- Inline elem

HTML code|View
-|-
`Text with <u>underlined part</u> and normal part.`|Text with <u>underlined part</u> and normal part.

---
