 # Markdown
- .md text file
- [Google Chrome Markdown Viewer extension](https://chrome.google.com/webstore/detail/markdown-viewer/ckkdlimhmcjmikdlpkmbgfkaikojcbjk)
  - Theme: GITHUB, AUTO
  - Compiler: REMARK breaks, gfm
  - Content: autoreload, syntax, toc 
- chrome://extensions/?id=ckkdlimhmcjmikdlpkmbgfkaikojcbjk
  - Hozzáférés automatikus engedélyezése a következő webhelyeken: BE
  - Engedélyezés inkognitó módban: BE
  - Fájl URL-ekhez való hozzáférés engedélyezése: BE

## Headings
- Automatically convert to link targets (just alphabetic characters and numbers, spaces to -)

|Markdown|HTML code|Output
|-|-|-
|`# Heading level 1`<br>OR<br>`Heading level 1`<br>`==`|\<h1>Heading level 1\</h1>|<h1>Heading level 1</h1>
|`## Heading level 2`<br>OR<br>`Heading level 2`<br>`--`|\<h2>Heading level 2\</h2>|<h2>Heading level 2</h2>
|`### Heading level 3`   |\<h3>Heading level 3\</h3>|<h3>Heading level 3</h3>
|`#### Heading level 4 ` |\<h4>Heading level 4\</h4>|<h4>Heading level 4</h4>
|`##### Heading level 5` |\<h5>Heading level 5\</h5>|<h5>Heading level 5</h5>
|`###### Heading level 6`|\<h6>Heading level 6\</h6>|<h6>Heading level 6</h6>

## Line Break

|Markdown|HTML code|Output
|-|-|-
|`text in a line`<br>`another text in another line`|text in a line\<br>another text in another line|text in a line<br>another text in another line

## Paragraphs

|Markdown|HTML code|Output
|-|-|-
|`text in a paragraph`<br><br>`text in another paragraph`|\<p>text in a paragraph\</p><br>\<p>text in another paragraph\</p>|<p>text in a paragraph</p><p>text in another paragraph</p>

## Text formats

|Markdown|HTML code|Output
|-|-|-
|`simple text`|\<p>simple text\</p>|<p>simple text</p>
|`_italic text_`|\<i>italic text\</i>|<i>italic text</i> 
|`**bold text**`|\<b>bold text\</b>|<b>bold text</b>
|`**_bold & italic text_**`|\<b>\<i>bold & italic text\</i>\</b>|<b><i>bold & italic text</i></b> 
|`~strike through text~`|\<s>strike through text\</s>|<s>strike through text</s>
|\``inline code`\`|\<code>inline code\</code>|`inline code`|
|`~~~`<br>`fenced code block`<br>`˝˝˝`||```fenced code block```
|`> block`<br>`>> nested block`<br>`>>> nested sub-block`|\<blockquote>block ...\</blockquote>|<blockquote>block<blockquote>nested block<blockquote>nested sub-block</blockquote></blockquote></blockquote>

## Lists

|Markdown|HTML code|Output
|-|-|-
|`- unordered list`<br>`  + unordered list`<br>`    * unordered list`|\<ul>\<li>unordered list\</li>...\</ul>|<ul><li>unordered list</li><ul><li>unordered list</li><ul><li>unordered list</li></ul></ul></ul>
|`1. ordered list`<br>`2. ordered list`<br>`3. ordered list`|\<ol>\<li>ordered list\</li>...\</ol>|<ol><li>ordered list</li><li>ordered list</li><li>ordered list</li></ol>

## Links
- Headings automatically convert to link targets (just alphabetic characters and numbers, spaces to -)

|Markdown|HTML code|Output
|-|-|-
|`https://www.google.com`|\<a href="`https://www.google.com`"><br>`https://www.google.com`\</a>|<a href="https://www.google.com">https://www.google.com</a>
|`[Back to section headings](#headings)`|\<a href="#headings">Back to section headings\</a>|<a href="#headings">Back to section headings</a>
|`[Link to README.md file in parent folder](../README.md)`|\<a href="../README.md">Link to README.md file in parent folder\</a>|<a href="../README.md">Link to README.md file in parent folder</a>
|`[Link to page.md file in a subfolder](./subfolder/page.md)`|\<a href="./subfolder/page.md">Link to page.md file in a subfolder\</a>|<a href="./subfolder/page.md">Link to page.md file in a subfolder</a>
|`![unreachable picture](sun.jpg)`|\<img src="sun.jpg" alt="unreachable picture">|<img src="sun.jpg" alt="unreachable picture">
|`![reachable picture](./subfolder/sun.jpg)`|\<img src="./subfolder/sun.jpg" alt="reachable picture">|<img src="./subfolder/sun.jpg" alt="reachable picture" width="50">
|`[![clickable picture](./subfolder/house%20icon.png)](#markdown)`|\<a href="#markdown">\<img src="./subfolder/house%20icon.png" alt="clickable picture">\</a>|<a href="#markdown"><img src="./subfolder/house%20icon.png" alt="clickable picture" width="50"></a>
|`Here is a simple footnote[^1].`<br>`[^1]: My reference.`||Here is a simple footnote[^1].
[^1]: My reference.

## Table
|ALIGN left (default)<br>&#124;`:-`&#124;|ALIGN center<br>&#124;`:-:`&#124;|ALIGN right<br>&#124;`-:`&#124;
:-|:-:|-:
left|center|right

## Tasks
`- [x] checked task`
- [x] checked task

`- [ ] unchecked task`
- [ ] unchecked task