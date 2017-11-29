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

####HTML Quotation and Citation Elements

| Tag            | Description                              |
| -------------- | ---------------------------------------- |
| `<abbr>`       | Defines an abbreviation or acronym       |
| `address`      | Defines contact information for the author/owner of a document |
| `bdo`          | Defines the text direction               |
| `<blockquote>` | Defines a section that is quoted from another source |
| `<cite>`       | Defines the title of a work              |
| `<q>`          | Defines a short inline quotation         |

### HTML Comments

####HTML Comment Tags

You can add comments to your HTML source by using the following syntax:

```html
<!-- Write your comments here -->
```

