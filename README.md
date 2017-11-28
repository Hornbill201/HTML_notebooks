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