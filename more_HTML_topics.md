# More Topics on HTML

## HTML Forms

### HTML Forms

#### The `<form>` Element

The HTML **`<form>`** element defines a form that is used to collect user input:

```html
<form>
  .
  form elements
  .
</form>
```

An HTML form contains **form elements**.

Form elements are different types of input elements, like text fields, checkboxes, radio buttons, submit buttons, and more.

## The `<input>` Element

The **`<input>`** element is the most important form element.

The `<input>` element can be displayed in several ways, depending on the **type** attribute.

Here are some examples:

| Type                    | Description                              |
| ----------------------- | ---------------------------------------- |
| `<input type="text">`   | Defines a one-line text input field      |
| `<input type="radio">`  | Defines a radio button (for selecting one of many choices) |
| `<input type="submit">` | Defines a submit button (for submitting the form) |

#### Text Input

**`<input type="text">`** defines a one-line input field for **text input**:

```html
<form>
  First name:<br>
  <input type="text" name="firstname"><br>
  Last name:<br>
  <input type="text" name="lastname">
</form>
```

#### Radio Button Input

**`<input type="radio">`** defines a **radio button**.

Radio buttons let a user select ONE of a limited number of choices:

```html
<form>
  <input type="radio" name="gender" value="male" checked> Male<br>
  <input type="radio" name="gender" value="female"> Female<br>
  <input type="radio" name="gender" value="other"> Other
</form>
```

#### The Submit Button

**`<input type="submit">`** defines a button for **submitting** the form data to a **form-handler**.

The form-handler is typically a server page with a script for processing input data.

The form-handler is specified in the form's **action** attribute:

```html
<form action="/action_page.php">
  First name:<br>
  <input type="text" name="firstname" value="Mickey"><br>
  Last name:<br>
  <input type="text" name="lastname" value="Mouse"><br><br>
  <input type="submit" value="Submit">
</form>
```

#### The Action Attribute

The **action** attribute defines the action to be performed when the form is submitted.

Normally, the form data is sent to a web page on the server when the user clicks on the submit button.

In the example above, the form data is sent to a page on the server called "/action_page.php". This page contains a server-side script that handles the form data:

```html
<form action="/action_page.php">
```

If the action attribute is omitted, the action is set to the current page.

#### The Target Attribute

The **target** attribute specifies if the submitted result will open in a new browser tab, a frame, or in the current window.

The default value is "**_self**" which means the form will be submitted in the current window.

To make the form result open in a new browser tab, use the value "**_blank**":

```html
<form action="/action_page.php" target="_blank">
```

Other legal values are "**_parent**", "**_top**", or a name representing the name of an iframe.

#### The Method Attribute

The **method** attribute specifies the HTTP method (**GET **or **POST**) to be used when submitting the form data:

```html
<form action="/action_page.php" method="get">
```

or

```html
<form action="/action_page.php" method="post">
```

#### When to Use GET?

The default method when submitting form data is GET.

However, when GET is used, the submitted form data will be **visible in the page address field**:

```html
/action_page.php?firstname=Mickey&lastname=Mouse
```

**Notes on GET:**

- Appends form-data into the URL in name/value pairs
- The length of a URL is limited (about 3000 characters)
- Never use GET to send sensitive data! (will be visible in the URL)
- Useful for form submissions where a user want to bookmark the result
- GET is better for non-secure data, like query strings in Google

#### When to Use POST?

Always use POST if the form data contains sensitive or personal information. The POST method does not display the submitted form data in the page address field.

**Notes on POST:**

- POST has no size limitations, and can be used to send large amounts of data.
- Form submissions with POST cannot be bookmarked

#### The Name Attribute

Each input field must have a **name** attribute to be submitted.

If the name attribute is omitted, the data of that input field will not be sent at all.

This example will only submit the "Last name" input field:

```html
<form action="/action_page.php">
  First name:<br>
  <input type="text" value="Mickey"><br>
  Last name:<br>
  <input type="text" name="lastname" value="Mouse"><br><br>
  <input type="submit" value="Submit">
</form>
```

#### Grouping Form Data with `<fieldset>`

The **`<fieldset>`** element is used to group related data in a form.

The **`<legend>`** element defines a caption for the `<fieldset>` element.

```html
<form action="/action_page.php">
  <fieldset>
    <legend>Personal information:</legend>
    First name:<br>
    <input type="text" name="firstname" value="Mickey"><br>
    Last name:<br>
    <input type="text" name="lastname" value="Mouse"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>
```

Here is the list of `<form>` attributes:

| Attribute      | Description                              |
| -------------- | ---------------------------------------- |
| accept-charset | Specifies the charset used in the submitted form (default: the page charset). |
| action         | Specifies an address (url) where to submit the form (default: the submitting page). |
| autocomplete   | Specifies if the browser should autocomplete the form (default: on). |
| enctype        | Specifies the encoding of the submitted data (default: is url-encoded). |
| method         | Specifies the HTTP method used when submitting the form (default: GET). |
| name           | Specifies a name used to identify the form (for DOM usage: document.forms.name). |
| novalidate     | Specifies that the browser should not validate the form. |
| target         | Specifies the target of the address in the action attribute (default: _self). |

### HTML Form Elements

This chapter describes all HTML form elements.

#### The `<input>` Element

The most important form element is the **`<input>`** element.

The `<input>` element can be displayed in several ways, depending on the **type** attribute.

```html
<input name="firstname" type="text">
```

If the **type **attribute is omitted, the input field gets the default type: "text".

All the different input types are covered in the next chapter.

#### The `<select>` Element

The **`<select>`** element defines a **drop-down list**:

```html
<select name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

The **`<option>`** elements defines an option that can be selected.

By default, the first item in the drop-down list is selected.

To define a pre-selected option, add the **selected** attribute to the option:

```html
<option value="fiat" selected>Fiat</option>
```

#### Visible Values:

Use the **size** attribute to specify the number of visible values:

```html
<select name="cars" size="3">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

#### Allow Multiple Selections:

Use the **multiple** attribute to allow the user to select more than one value:

```html
<select name="cars" size="4" multiple>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

#### The `<textarea>` Element

The **`<textarea>`** element defines a multi-line input field (**a text area**):

```html
<textarea name="message" rows="10" cols="30">
The cat was playing in the garden.
</textarea>
```

The **rows** attribute specifies the visible number of lines in a text area.

The **cols** attribute specifies the visible width of a text area.

You can also define the size of the text area by using CSS:

```html
<textarea name="message" style="width:200px; height:600px">
The cat was playing in the garden.
</textarea>
```

#### The `<button>` Element

The **`<button>`** element defines a clickable **button**:

```html
<button type="button" onclick="alert('Hello World!')">Click Me!</button>
```

#### HTML5 Form Elements

HTML5 added the following form elements:

- `<datalist>`
- `<output>`

**Note:** Browsers do not display unknown elements. New elements that are not supported in older browsers will not "destroy" your web page.

#### HTML5 `<datalist>` Element

The **`<datalist>`** element specifies a list of pre-defined options for an `<input>` element.

Users will see a drop-down list of the pre-defined options as they input data.

The **list** attribute of the `<input>` element, must refer to the **id** attribute of the `<datalist>` element.

```html
<form action="/action_page.php">
  <input list="browsers">
  <datalist id="browsers">
    <option value="Internet Explorer">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist> 
</form>
```

#### HTML5 `<output>` Element

The `<output>` element represents the result of a calculation (like one performed by a script).

Perform a calculation and show the result in an `<output>` element:
```html
<form action="/action_page.php"
  oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  0
  <input type="range"  id="a" name="a" value="50">
  100 +
  <input type="number" id="b" name="b" value="50">
  =
  <output name="x" for="a b"></output>
  <br><br>
  <input type="submit">
</form>
```



####  HTML Form Elements

| Tag          | Description                              |
| ------------ | ---------------------------------------- |
| `<form>`     | Defines an HTML form for user input      |
| `<input>`    | Defines an input control                 |
| `<textarea>` | Defines a multiline input control (text area) |
| `<label>`    | Defines a label for an `<input>` element |
| `<fieldset>` | Groups related elements in a form        |
| `<legend>`   | Defines a caption for a `<fieldset>` element |
| `<select>`   | Defines a drop-down list                 |
| `<optgroup>` | Defines a group of related options in a drop-down list |
| `<option>`   | Defines an option in a drop-down list    |
| `<button>`   | Defines a clickable button               |
| `<datalist>` | Specifies a list of pre-defined options for input controls (HTML5) |
| `<output>`   | Defines the result of a calculation (HTML5) |

