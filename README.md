# HTML notebooks
This is the Notebook of HTML from w3schools. 

## A Simple HTML Document

```html
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

Example Explained

* The `<!DOCTYPE html>` declaration defines this document to be HTML5
* The `<html>` element is the root element of an HTML page
* The `<head>` element contains meta information about the document
* The `<title>` element specifies a title for the document
* The `<body>` element contains the visible page content
* The `<h1>` element defines a large heading
* The `<p>` element defines a paragraph

### HTML Documents

All HTML documents must start with a document type declaration: ``<!DOCTYPE html>``.

The HTML document itself begins with ``<html>`` and ends with ``</html>``.

The visible part of the HTML document is between ``<body>`` and ``</body>``.

### HTML Headings

HTML headings are defined with the `<h1>` to ``<h6>`` tags.

``<h1>`` defines the most important heading. ``<h6>`` defines the least important heading.

### HTML Paragraphs

HTML paragraphs are defined with the ``<p>``tag.

### HTML Links

HTML links are defined with the ``<a>`` tag:

Example:

```html
<a href="https://www.w3schools.com">This is a link</a>
```

The link's destination is specified in the **href attribute**. 

Attributes are used to provide additional information about HTML elements.

### HTML Images

HTML images are defined with the ``<img>`` tag.

The source file (src), alternative text (alt), width, and height are provided as attributes:

Example:

```html
<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">
```

### Do Not Forget the End Tag

Some HTML elements will display correctly, even if you forget the end tag.

**Never rely on this. It might produce unexpected results and/or errors if you forget the end tag.**

### Empty HTML Elements

HTML elements with no content are called empty elements.

``<br>`` is an empty element without a closing tag (the ``<br>`` tag defines a line break).

Empty elements can be "closed" in the opening tag like this: ``<br />``.

HTML5 does not require empty elements to be closed. But if you want stricter validation, or if you need to make your document readable by XML parsers, you must close all HTML elements properly.

### HTML Attributes

- All HTML elements can have **attributes**
- Attributes provide **additional information** about an element
- Attributes are always specified in **the start tag**
- Attributes usually come in name/value pairs like: ``name="value"``

Examples:

```html
<a href="https://www.w3schools.com">This is a link</a>
<img src="img_girl.jpg">
<img src="img_girl.jpg" width="500" height="600">
<img src="img_girl.jpg" alt="Girl with a jacket">
<p> The alt attribute specifies an alternative text to be used, when an image cannot be displayed. </p>

<p style="color:red">I am a paragraph</p>
```

The language of the document can be declared in the **<html>** tag.

The language is declared with the **lang** attribute.

Declaring a language is important for accessibility applications (screen readers) and search engines:

```html
<!DOCTYPE html>
<html lang="en-US">
<body>

...

</body>
</html>
```

A **title** attribute is added to the ``<p>`` element. The value of the title attribute will be displayed as a tooltip when you mouse over the paragraph:

```html
<p title="I'm a tooltip">
This is a paragraph.
</p>
```

We Suggest: Use Lowercase Attributes 

The HTML5 standard does not require lowercase attribute names.

The title attribute can be written with uppercase or lowercase like **title** or **TITLE**.

W3C **recommends** lowercase in HTML, and **demands** lowercase for stricter document types like XHTML.

W3C **recommends** quotes in HTML, and **demands** quotes for stricter document types like XHTML.

Sometimes it is **necessary** to use quotes. This example will not display the title attribute correctly, because it contains a space.

### Chapter Summary

- All HTML elements can have **attributes**
- The **title** attribute provides additional "tool-tip" information
- The **href** attribute provides address information for links
- The **width** and **height** attributes provide size information for images
- The **alt** attribute provides text for screen readers
- At W3Schools we always use **lowercase** attribute names
- At W3Schools we always **quote** attribute values with double quotes

Below is an alphabetical list of some attributes often used in HTML:

| Attribute | Description                              |
| --------- | ---------------------------------------- |
| alt       | Specifies an alternative text for an image, when the image cannot be displayed |
| disabled  | Specifies that an input element should be disabled |
| href      | Specifies the URL (web address) for a link |
| id        | Specifies a unique id for an element     |
| src       | Specifies the URL (web address) for an image |
| style     | Specifies an inline CSS style for an element |
| title     | Specifies extra information about an element (displayed as a tool tip) |

A complete list of all attributes for each HTML element, is listed in our: [HTML Attribute Reference](https://www.w3schools.com/tags/ref_attributes.asp).

### Headings

---

Headings are defined with the ``<h1>`` to ``<h6>`` tags.

``<h1>`` defines the most important heading. ``<h6>`` defines the least important heading.

Example

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

####  Bigger Headings

Each HTML heading has a default size. However, you can specify the size for any heading with the style attribute:

```html
<h1 style="font-size:60px;">Heading 1</h1>
```

#### HTML Horizontal Rules

The ``<hr>`` tag defines a thematic break in an HTML page, and is most often displayed as a horizontal rule.

The ``<hr>`` element is used to separate content (or define a change) in an HTML page:

```html
<h1>This is heading 1</h1>
<p>This is some text.</p>
<hr>
<h2>This is heading 2</h2>
<p>This is some other text.</p>
<hr>
```

#### The HTML `<head>` Element

The HTML ``<head>`` element has nothing to do with HTML headings.

The ``<head>`` element is a container for metadata. HTML metadata is data about the HTML document. Metadata is not displayed.

The ``<head>`` element is placed between the ``<html>`` tag and the ``<body>`` tag:

```html
<!DOCTYPE html>
<html>

<head>
  <title>My First HTML</title>
  <meta charset="UTF-8">
</head>

<body>
...
```

#### HTML Tag Reference

| Tag              | Description                              |
| ---------------- | ---------------------------------------- |
| `<html>`         | Defines the root of an HTML document     |
| `<body>`         | Defines the document's body              |
| `<head>`         | A container for all the head elements (title, scripts, styles, meta information, and more) |
| `<h1>` to `<h6>` | Defines HTML headings                    |
| `<hr>`           | Defines a thematic change in the content |

### HTML Paragraphs

---

#### HTML Display

You cannot be sure how HTML will be displayed.

Large or small screens, and resized windows will create different results.

With HTML, you cannot change the output by adding extra spaces or extra lines in your HTML code.

#### HTML Line Breaks

The HTML ``<br>`` element defines a **line break**.

Use ``<br>`` if you want a line break (a new line) without starting a new paragraph:

```html
<p>This is<br>a paragraph<br>with line breaks.</p>
```

#### The HTML ``<pre>`` Element

The HTML ``<pre>`` element defines preformatted text.

The text inside a ``<pre>`` element is displayed in a fixed-width font (usually Courier), and it preserves both spaces and line breaks:

```html
<pre>
  My Bonnie lies over the ocean.

  My Bonnie lies over the sea.

  My Bonnie lies over the ocean.

  Oh, bring back my Bonnie to me.
</pre>
```

####  HTML Tag Reference

| Tag     | Description                 |
| ------- | --------------------------- |
| `<p>`   | Defines a paragraph         |
| `<br>`  | Inserts a single line break |
| `<pre>` | Defines pre-formatted text  |

### HTML Styles

#### The HTML Style Attribute

Setting the style of an HTML element, can be done with the **style attribute**.

The HTML style attribute has the following **syntax**:

```html
<tagname style="property:value;">
```

The ***property*** is a CSS property. The ***value*** is a CSS value.

#### HTML Background Color

The **background-color** property defines the background color for an HTML element.

This example sets the background color for a page to powderblue:

```html
<body style="background-color:powderblue;">
<h1>This is a heading</h1>
<p>This is a paragraph.</p>
</body>
```

#### HTML Text Color

The **color** property defines the text color for an HTML element:

```html
<h1 style="color:blue;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>
```

#### HTML Fonts

The **font-family** property defines the font to be used for an HTML element:

```html
<h1 style="font-family:verdana;">This is a heading</h1>
<p style="font-family:courier;">This is a paragraph.</p>
```

#### HTML Text Size

The **font-size** property defines the text size for an HTML element:

```html
<h1 style="font-size:300%;">This is a heading</h1>
<p style="font-size:160%;">This is a paragraph.</p>
```

#### HTML Text Alignment

The **text-align** property defines the horizontal text alignment for an HTML element:

```html
<h1 style="text-align:center;">Centered Heading</h1>
<p style="text-align:center;">Centered paragraph.</p>
```

#### Chapter Summary

- Use the **style** attribute for styling HTML elements
- Use **background-color** for background color
- Use **color** for text colors
- Use **font-family** for text fonts
- Use **font-size** for text sizes
- Use **text-align** for text alignment

### HTML Text Formatting

---

HTML also defines special **elements** for defining text with a special **meaning**.

HTML uses elements like ``<b>`` and ``<i>`` for formatting output, like **bold** or *italic* text.

Formatting elements were designed to display special types of text:

- ``<b>`` - Bold text
- ``<strong>`` - Important text
- ``<i>`` - Italic text
- ``<em>`` - Emphasized text
- ``<mark>`` - Marked text
- ``<small>`` - Small text
- ``<del>`` - Deleted text
- ``<ins>`` - Inserted text
- ``<sub>`` - Subscript text
- ``<sup>`` - Superscript text

### HTML Quotation and Citation Elements

#### HTML `<q>` for Short Quotations

The HTML ``<q>`` element defines a short quotation.

Browsers usually insert quotation marks around the ``<q>`` element.

```html
<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
```

#### HTML `<blockquote>` for Quotations

The HTML ``<blockquote>`` element defines a section that is quoted from another source.

Browsers usually indent ``<blockquote>`` elements.

```html
<p>Here is a quote from WWF's website:</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature.
The world's leading conservation organization,
WWF works in 100 countries and is supported by
1.2 million members in the United States and
close to 5 million globally.
</blockquote>
```

#### HTML `<abbr>` for Abbreviations

The HTML ``<abbr>`` element defines an abbreviation or an acronym.

Marking abbreviations can give useful information to browsers, translation systems and search-engines.

```html
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
```

#### HTML `<address>` for Contact Information

The HTML ``<address>`` element defines contact information (author/owner) of a document or an article.

The ``<address>`` element is usually displayed in italic. Most browsers will add a line break before and after the element.

```html
<address>
Written by John Doe.<br> 
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>
```

#### HTML `<cite>` for Work Title

The HTML ``<cite>`` element defines the title of a work.

Browsers usually display ``<cite>`` elements in italic.

```html
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```

#### HTML `<bdo>` for Bi-Directional Override

The HTML ``<bdo>`` element defines bi-directional override.

The ``<bdo>`` element is used to override the current text direction:

```html
<bdo dir="rtl">This text will be written from right to left</bdo>
```

#### HTML Quotation and Citation Elements

| Tag            | Description                              |
| -------------- | ---------------------------------------- |
| `<abbr>`       | Defines an abbreviation or acronym       |
| `address`      | Defines contact information for the author/owner of a document |
| `bdo`          | Defines the text direction               |
| `<blockquote>` | Defines a section that is quoted from another source |
| `<cite>`       | Defines the title of a work              |
| `<q>`          | Defines a short inline quotation         |

### HTML Comments

---

#### HTML Comment Tags

You can add comments to your HTML source by using the following syntax:

```html
<!-- Write your comments here -->
```

### HTML Styles - CSS

#### Styling HTML with CSS

**CSS** stands for **C**ascading **S**tyle **S**heets.

CSS describes **how HTML elements are to be displayed on screen, paper, or in other media**.

CSS **saves a lot of work**. It can control the layout of multiple web pages all at once.

CSS can be added to HTML elements in 3 ways:

- **Inline** - by using the style attribute in HTML elements
- **Internal** - by using a `<style>` element in the `<head>` section
- **External** - by using an external CSS file

#### Inline CSS

An inline CSS is used to apply a unique style to a single HTML element.

An inline CSS uses the style attribute of an HTML element.

This example sets the text color of the <h1> element to blue:

```html
<h1 style="color:blue;">This is a Blue Heading</h1>
```

#### Internal CSS

An internal CSS is used to define a style for a single HTML page.

An internal CSS is defined in the `<head>` section of an HTML page, within a `<style>` element:

```html
<!DOCTYPE html>
<html>
<head>
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

#### External CSS

An external style sheet is used to define the style for many HTML pages.

**With an external style sheet, you can change the look of an entire web site, by changing one file!**

To use an external style sheet, add a link to it in the `<head>` section of the HTML page:

```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

An external style sheet can be written in any text editor. The file must not contain any HTML code, and must be saved with a .css extension.

Here is how the "styles.css" looks:

```css
body {
    background-color: powderblue;
}
h1 {
    color: blue;
}
p {
    color: red;
}
```

#### CSS Fonts

The CSS **color** property defines the text color to be used.

The CSS **font-family** property defines the font to be used.

The CSS **font-size **property defines the text size to be used.

```html
<!DOCTYPE html>
<html>
<head>
<style>
h1 {
    color: blue;
    font-family: verdana;
    font-size: 300%;
}
p  {
    color: red;
    font-family: courier;
    font-size: 160%;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

#### CSS Border

The CSS **border** property defines a border around an HTML element:

```html
p {
    border: 1px solid powderblue;
}
```

#### CSS Padding

The CSS **padding** property defines a padding (space) between the text and the border:

```html
p {
    border: 1px solid powderblue;
    padding: 30px;
}
```

#### CSS Margin

The CSS **margin** property defines a margin (space) **outside** the border:

```html
p {
    border: 1px solid powderblue;
    margin: 50px;
}
```

#### The id Attribute

To define a specific style for one special element, add an id attribute to the element:

```html
<p id="p01">I am different</p>
```

then define a style for the element with the specific id:

```html
#p01 {
    color: blue;
}
```

#### The class Attribute

To define a style for a special type of elements, add a class attribute to the element:

```html
<p class="error">I am different</p>
```

then define a style for the elements with the specific class:

```html
p.error {
    color: red;
}
```

#### External References

External style sheets can be referenced with a full URL or with a path relative to the current web page.

This example uses a full URL to link to a style sheet:

```html
<link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
```

This example links to a style sheet located in the html folder on the current web site:

```html
<link rel="stylesheet" href="/html/styles.css">
```

This example links to a style sheet located in the same folder as the current page:

```html
<link rel="stylesheet" href="styles.css">
```

#### Chapter Summary

- Use the HTML **style** attribute for inline styling
- Use the HTML **`<style>`** element to define internal CSS
- Use the HTML **`<link>`** element to refer to an external CSS file
- Use the HTML **`<head>`** element to store `<style>` and `<link>` elements
- Use the CSS **color** property for text colors
- Use the CSS **font-family** property for text fonts
- Use the CSS **font-size** property for text sizes
- Use the CSS **border** property for borders
- Use the CSS **padding** property for space inside the border
- Use the CSS **margin** property for space outside the border

### HTML Links

---

#### HTML Links

HTML links are hyperlinks.

You can click on a link and jump to another document.

When you move the mouse over a link, the mouse arrow will turn into a little hand.

```html
<a href="https://www.w3schools.com/html/">Visit our HTML tutorial</a>
```

#### Local Links

The example above used an absolute URL (A full web address).

A local link (link to the same web site) is specified with a relative URL (without http://www....).

```html
<a href="html_images.asp">HTML Images</a>
```

#### HTML Link Colors

By default, a link will appear like this (in all browsers):

- An unvisited link is underlined and blue
- A visited link is underlined and purple
- An active link is underlined and red

You can change the default colors, by using styles:

```html
<style>
a:link {
    color: green; 
    background-color: transparent; 
    text-decoration: none;
}

a:visited {
    color: pink;
    background-color: transparent;
    text-decoration: none;
}

a:hover {
    color: red;
    background-color: transparent;
    text-decoration: underline;
}

a:active {
    color: yellow;
    background-color: transparent;
    text-decoration: underline;
}
</style>
```

#### HTML Links - The target Attribute

The **target** attribute specifies where to open the linked document.

The target attribute can have one of the following values:

- _blank - Opens the linked document in a new window or tab
- _self - Opens the linked document in the same window/tab as it was clicked (this is default)
- _parent - Opens the linked document in the parent frame
- _top - Opens the linked document in the full body of the window
- framename - Opens the linked document in a named frame

This example will open the linked document in a new browser window/tab:

```html
<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
```

**Tip:** If your webpage is locked in a frame, you can use target="_top" to break out of the frame:

```html
<a href="https://www.w3schools.com/html/" target="_top">HTML5 tutorial!</a>
```

#### HTML Links - Image as Link

It is common to use images as links:

```html
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;border:0;">
</a>
```

#### HTML Links - Create a Bookmark

 HTML bookmarks are used to allow readers to jump to specific parts of a Web page.

Bookmarks can be useful if your webpage is very long.

To make a bookmark, you must first create the bookmark, and then add a link to it.

When the link is clicked, the page will scroll to the location with the bookmark.

First, create a bookmark with the id attribute:

Then, add a link to the bookmark ("Jump to Chapter 4"), from within the same page:

```html
<h2 id="C4">Chapter 4</h2>
<a href="#C4">Jump to Chapter 4</a>
```

Or, add a link to the bookmark ("Jump to Chapter 4"), from another page:

```html
<a href="html_demo.html#C4">Jump to Chapter 4</a>
```

#### External Paths

External pages can be referenced with a full URL or with a path relative to the current web page.

This example uses a full URL to link to a web page:

```html
<a href="https://www.w3schools.com/html/default.asp">HTML tutorial</a>
```

This example links to a page located in the html folder on the current web site:

```html
<a href="/html/default.asp">HTML tutorial</a>
```

This example links to a page located in the same folder as the current page:

```html
<a href="default.asp">HTML tutorial</a>
```

#### Remove the underline from the link

```html
<a href="html_images.asp" target="_blank" style="text-decoration:none">HTML Images</a>
```

#### Chapter Summary

- Use the **`<a>`** element to define a link
- Use the **href** attribute to define the link address
- Use the **target** attribute to define where to open the linked document
- Use the **`<img>`** element (inside `<a>`) to use an image as a link
- Use the **id** attribute (id="*value*") to define bookmarks in a page
- Use the **href** attribute (href="#*value*") to link to the bookmark

### HTML Images

```html
<img src="pulpitrock.jpg" alt="Mountain View">
```

#### Image Size - Width and Height

You can use the **style** attribute to specify the width and height of an image.

```html
<img src="img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">
```

Alternatively, you can use the **width** and **height** attributes:

```html
<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
```

However, we suggest using the style attribute. It prevents styles sheets from changing the size of images:

```html
<!DOCTYPE html>
<html>
<head>
<style>
img { 
    width:100%; 
}
</style>
</head>
<body>

<img src="html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
<img src="html5.gif" alt="HTML5 Icon" width="128" height="128">

</body>
</html>
```

#### Image as a Link

 To use an image as a link, put the `<img>` tag inside the `<a>` tag:

```html
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;border:0;">
</a>
```

#### Image Floating

Use the CSS **float** property to let the image float to the right or to the left of a text:

```html
<p><img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
The image will float to the right of the text.</p>

<p><img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">
The image will float to the left of the text.</p>
```

#### Image Maps

Use the `<map>` tag to define an image-map. An image-map is an image with clickable areas.

In the image below, click on the computer, the phone, or the cup of coffee:

```html
<img src="workplace.jpg" alt="Workplace" usemap="#workmap">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
  <area shape="circle" coords="337,300,44" alt="Coffee" href="coffee.htm">
</map>
```

The name attribute of the `<map>` tag is associated with the `<img>`'s usemap attribute and creates a relationship between the image and the map.

The `<map>` tag contains a number of `<area>` tags, that defines the clickable areas in the image-map.

#### Background Image

To add a background image on an HTML element, use the CSS property `background-image`:

```html
<body style="background-image:url('clouds.jpg')">
<h2>Background Image</h2>
</body>
```

To add a background image on a paragraph, specify the background-image property on the P element:

```html
<body>

<p style="background-image:url('clouds.jpg')">
...
</p>

</body>
```

#### The `<picture>` Element

HTML5 introduced the `<picture>` element to add more flexibility when specifying image resources.

The `<picture>` element contains a number of `<source>` elements, each referring to different image sources. This way the browser can choose the image that best fit the current view and/or device.

Each `<source>` element have attributes describing when their image is the most suitable.

The browser will use the first `<source>` element with matching attribute values, and ignore any following `<source>` elements.

Show one picture if the browser window (viewport) is a minimum of 650 pixels, and another image if not, but larger than 465 pixels.

```html
<picture>
<source media="(min-width: 650px)" srcset="img_pink_flowers.jpg">
<source media="(min-width: 465px)" srcset="img_white_flower.jpg">
<img src="img_orange_flowers.jpg" alt="Flowers" style="width:auto;">
</picture>
```

**Note:** Always specify an `<img>` element as the last child element of the `<picture>` element. The `<img>` element is used by browsers that to not support the `<picture>` element, or if none of the `<source>` tags matched.

#### HTML Screen Readers

A screen reader is a software program that reads the HTML code, converts the text, and allows the user to "listen" to the content. Screen readers are useful for people who are blind, visually impaired, or learning disabled.

#### Chapter Summary

- Use the HTML **`<img>`** element to define an image
- Use the HTML **src** attribute to define the URL of the image
- Use the HTML **alt** attribute to define an alternate text for an image, if it cannot be displayed
- Use the HTML **width** and **height** attributes to define the size of the image
- Use the CSS **width** and **height** properties to define the size of the image (alternatively)
- Use the CSS **float** property to let the image float
- Use the HTML **`<map>`** element to define an image-map
- Use the HTML **`<area>`** element to define the clickable areas in the image-map
- Use the HTML `<img>`'s element **usemap** attribute to point to an image-map
- Use the HTML **`<picture>`** element to show different images for different devices


### HTML Tables

---

#### Defining an HTML Table

An HTML table is defined with the **`<table>`** tag.

Each table row is defined with the **`<tr>`** tag. A table header is defined with the **`<th>`** tag. By default, table headings are bold and centered. A table data/cell is defined with the **`<td>`** tag.

```html
<table style="width:100%">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th> 
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td> 
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td> 
    <td>94</td>
  </tr>
</table>
```

**Note:** The `<td>` elements are the data containers of the table.
They can contain all sorts of HTML elements; text, images, lists, other tables, etc.

#### HTML Table - Adding a Border

If you do not specify a border for the table, it will be displayed without borders.

A border is set using the CSS **border** property:

```html
table, th, td {
    border: 1px solid black;
}
```

#### HTML Table - Collapsed Borders

If you want the borders to collapse into one border, add the CSS **border-collapse** property:

```html
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
```

#### HTML Table - Adding Cell Padding

Cell padding specifies the space between the cell content and its borders.

If you do not specify a padding, the table cells will be displayed without padding.

To set the padding, use the CSS **padding** property:

```html
th, td {
    padding: 15px;
}
```

#### HTML Table - Left-align Headings

By default, table headings are bold and centered.

To left-align the table headings, use the CSS **text-align** property:

```html
th {
    text-align: left;
}
```

**Note: All these boarder, padding should be included in the `<style>` attribute. **

#### HTML Table - Adding Border Spacing

Border spacing specifies the space between the cells.

To set the border spacing for a table, use the CSS **border-spacing** property:

```html
table {
    border-spacing: 5px;
}
```

#### HTML Table - Cells that Span Many Columns

To make a cell span more than one column, use the **colspan** attribute:

```html
<table style="width:100%">
  <tr>
    <th>Name</th>
    <th colspan="2">Telephone</th>
  </tr>
  <tr>
    <td>Bill Gates</td>
    <td>55577854</td>
    <td>55577855</td>
  </tr>
</table>
```

#### HTML Table - Cells that Span Many Rows

```html
<table style="width:100%">
  <tr>
    <th>Name:</th>
    <td>Bill Gates</td>
  </tr>
  <tr>
    <th rowspan="2">Telephone:</th>
    <td>55577854</td>
  </tr>
  <tr>
    <td>55577855</td>
  </tr>
</table>
```

#### HTML Table - Adding a Caption

```html
<table style="width:100%">
  <caption>Monthly savings</caption>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$50</td>
  </tr>
</table>
```

**Note:** The `<caption>` tag must be inserted immediately after the `<table>` tag.

#### A Special Style for One Table

To define a special style for a special table, add an **id** attribute to the table:

```html
table#t01 {
    width: 100%; 
    background-color: #f1f1c1;
}
```

```html
<table id="t01">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th> 
    <th>Age</th>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td> 
    <td>94</td>
  </tr>
</table>
```

**Add more styles**

```html
table#t01 tr:nth-child(even) {
    background-color: #eee;
}
table#t01 tr:nth-child(odd) {
    background-color: #fff;
}
table#t01 th {
    color: white;
    background-color: black;
}
```

#### Chapter Summary

- Use the HTML **`<table>`** element to define a table
- Use the HTML **`<tr>`** element to define a table row
- Use the HTML **`<td>`** element to define a table data
- Use the HTML **`<th>`** element to define a table heading
- Use the HTML **`<caption>`** element to define a table caption
- Use the CSS **border** property to define a border
- Use the CSS **border-collapse** property to collapse cell borders
- Use the CSS **padding** property to add padding to cells
- Use the CSS **text-align** property to align cell text
- Use the CSS **border-spacing** property to set the spacing between cells
- Use the **colspan** attribute to make a cell span many columns
- Use the **rowspan** attribute to make a cell span many rows
- Use the **id** attribute to uniquely define one table

### HTML Lists

#### Unordered HTML List

An unordered list starts with the **`<ul>`** tag. Each list item starts with the **`<li>`** tag.

The list items will be marked with bullets (small black circles) by default:

```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

Unordered HTML List - Choose List Item Marker

The CSS **list-style-type** property is used to define the style of the list item marker:

| Value  | Description                              |
| ------ | ---------------------------------------- |
| disc   | Sets the list item marker to a bullet (default) |
| circle | Sets the list item marker to a circle    |
| square | Sets the list item marker to a square    |
| none   | The list items will not be marked        |

```html
<ul style="list-style-type:disc">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

#### Ordered HTML List

An ordered list starts with the **`<ol>`** tag. Each list item starts with the **`<li>`** tag.

The list items will be marked with numbers by default:

```html
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

#### Ordered HTML List - The Type Attribute

The **type** attribute of the `<ol>` tag, defines the type of the list item marker:

| Type     | Description                              |
| -------- | ---------------------------------------- |
| type="1" | The list items will be numbered with numbers (default) |
| type="A" | The list items will be numbered with uppercase letters |
| type="a" | The list items will be numbered with lowercase letters |
| type="I" | The list items will be numbered with uppercase roman numbers |
| type="i" | The list items will be numbered with lowercase roman numbers |

```html
<ol type="1">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

#### HTML Description Lists

HTML also supports description lists.

A description list is a list of terms, with a description of each term.

The **`<dl>`** tag defines the description list, the **`<dt>`** tag defines the term (name), and the **`<dd>`** tag describes each term: 

```html
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```

#### Nested HTML Lists

List can be nested (lists inside lists):

```html
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
```

#### Horizontal Lists

HTML lists can be styled in many different ways with CSS.

One popular way is to style a list horizontally, to create a menu:

```html
<!DOCTYPE html>
<html>
<head>
<style>
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333333;
}

li {
    float: left;
}

li a {
    display: block;
    color: white;
    text-align: center;
    padding: 16px;
    text-decoration: none;
}

li a:hover {
    background-color: #111111;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
```

#### Chapter Summary

- Use the HTML **`<ul>`** element to define an unordered list
- Use the CSS **list-style-type** property to define the list item marker
- Use the HTML **`<ol>`** element to define an ordered list
- Use the HTML **type** attribute to define the numbering type
- Use the HTML **`<li>`** element to define a list item
- Use the HTML **`<dl>`** element to define a description list
- Use the HTML **`<dt>`** element to define the description term
- Use the HTML **`<dd>`** element to describe the term in a description list
- Lists can be nested inside lists
- List items can contain other HTML elements
- Use the CSS property **float:left** or **display:inline **to display a list horizontally

### HTML Block and Inline Elements

Every HTML element has a default display value depending on what type of element it is. The default display value for most elements is block or inline.

The `<div>` element is a block-level element.

```html
<div>Hello</div>
<div>World</div>
```

Inline elements in HTML:

```html
<a> <abbr> <acronym> <b> <bdo>
<big> <br> <button> <cite> <code>
<dfn> <em> <i> <img> <input> 
<kbd> <label> <map> <object> <q> 
<samp> <script> <select> <small> <span> 
<strong> <sub> <sup> <textarea> <time> <tt> <var>
```

#### The `<div>` Element

The `<div>` element is often used as a container for other HTML elements.

The `<div>` element has no required attributes, but both **style** and **class** are common.

When used together with CSS, the `<div>` element can be used to style blocks of content:

```html
<div style="background-color:black;color:white;padding:20px;">
  <h2>London</h2>
  <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
</div>
```

### The `<span>` Element

The `<span>` element is often used as a container for some text.

The `<span>` element has no required attributes, but both **style** and **class** are common.

When used together with CSS, the `<span>` element can be used to style parts of the text:

```html
<h1>My <span style="color:red">Important</span> Heading</h1>
```

