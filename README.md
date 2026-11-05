# 🚀 Session 4 – HTML Practice Project

## 📖 1. Project Overview

This is an educational, beginner-level project designed to practice and master fundamental **HTML5 concepts**.

The main goal is to build a well-structured webpage using pure HTML, without using CSS for styling or JavaScript for interactivity.

The project focuses on the structural elements of web development, including:

* HTML document structure.
* Headings and text formatting.
* Hyperlinks and navigation.
* Images and media embedding.
* Ordered, unordered, and description lists.
* Tables and cell merging.
* HTML forms and input elements.
* Form submission and navigation.

---

## 📁 2. Project Structure

```text
📦 Session-4-HTML-Practice
 ┣ 📂 img/
 ┃ ┣ 📜 001 (1).jpg
 ┃ ┗ 📜 003.jpg
 ┣ 📜 index.html
 ┣ 📜 About.html
 ┣ 📜 Login.html
 ┗ 📜 Register.html
```

### File Description

| File / Folder   | Description                                                 |
| --------------- | ----------------------------------------------------------- |
| `index.html`    | Main page containing the HTML elements and practice form.   |
| `About.html`    | Secondary page demonstrating internal navigation and lists. |
| `Login.html`    | Dummy destination page for the Login button.                |
| `Register.html` | Dummy destination page for the Registration button.         |
| `img/`          | Contains the images used in the project.                    |

---

## 🛠️ 3. HTML Concepts Used

### 3.1 Basic HTML Structure

| Tag / Attribute          | Description                                              |
| ------------------------ | -------------------------------------------------------- |
| `<!DOCTYPE html>`        | Declares the document as HTML5.                          |
| `<html>`                 | Root element of the webpage.                             |
| `<head>`                 | Contains document metadata.                              |
| `<meta charset="UTF-8">` | Supports different characters and languages.             |
| `<meta name="viewport">` | Helps control the page layout on different screen sizes. |
| `<title>`                | Sets the browser tab title.                              |
| `<body>`                 | Contains all visible webpage content.                    |

### 3.2 Headings and Paragraphs

* `<h1>` to `<h6>`: Define headings with different levels of importance.
* `<p>`: Defines a paragraph.
* `<strong>`: Indicates important text, usually displayed in bold.
* `<hr>`: Creates a thematic break between sections.
* `<br>`: Inserts a line break.
* `<center>`: Centers content. This is an obsolete HTML element, included here for educational purposes.

### 3.3 Links and Navigation

The `<a>` (Anchor) tag is used to create hyperlinks.

**Types of Links:**

* **Internal Links:** Navigate between project pages.

  ```html
  <a href="About.html">About Us</a>
  ```

* **External Links:** Navigate to external websites.

  ```html
  <a href="https://www.google.com">Google</a>
  ```

* **Target Attribute:** Opens a link in a new tab.

  ```html
  target="_blank"
  ```

* **Email Links:** Open the default email application.

  ```html
  <a href="mailto:example@email.com">Send Email</a>
  ```

* **Phone Links:** Allow users to initiate a phone call on supported devices.

  ```html
  <a href="tel:+201000000000">Call Us</a>
  ```

* **WhatsApp and Telegram Links:**

  ```html
  https://wa.me/
  https://t.me/
  ```

### 3.4 Images and Image Paths

The `<img>` tag is used to embed images.

| Attribute | Description               |
| --------- | ------------------------- |
| `src`     | Specifies the image path. |
| `width`   | Sets the image width.     |
| `height`  | Sets the image height.    |

Example:

```html
<img src="img/003.jpg" width="300" height="200">
```

### 3.5 HTML Lists

**Ordered Lists (`<ol>`):**

Used to display numbered or alphabetically ordered items.

```html
<ol type="a">
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ol>
```

**Unordered Lists (`<ul>`):**

Used to display bulleted items.

```html
<ul>
    <li>Programming</li>
    <li>Technology</li>
</ul>
```

**List Items (`<li>`):**

Define individual items inside ordered and unordered lists.

**Description Lists (`<dl>`):**

Used to display terms and their descriptions.

* `<dl>`: Defines the description list.
* `<dt>`: Defines the term.
* `<dd>`: Defines the description.

### 3.6 HTML Tables

Tables organize information into rows and columns.

| Tag / Attribute | Description                                   |
| --------------- | --------------------------------------------- |
| `<table>`       | Creates a table.                              |
| `<caption>`     | Adds a table title.                           |
| `<tr>`          | Defines a table row.                          |
| `<th>`          | Defines a header cell.                        |
| `<td>`          | Defines a standard data cell.                 |
| `border`        | Sets the table border width.                  |
| `rowspan`       | Merges cells vertically across multiple rows. |

**Example of Rowspan:**

```html
<td rowspan="2">Gaber</td>
```

This merges two cells vertically into one.

---

## 📝 4. Forms, Fieldsets, and Inputs

The `<form>` element is used to collect information from users.

### 4.1 Form Structure Elements

| Element      | Description                          |
| ------------ | ------------------------------------ |
| `<form>`     | Creates the form container.          |
| `<fieldset>` | Groups related form elements.        |
| `<legend>`   | Defines a caption for a fieldset.    |
| `<label>`    | Provides a description for an input. |

**Label and Input Connection:**

```html
<label for="username">Username:</label>
<input type="text" id="username" name="username">
```

The `for` attribute connects the label to the input through its `id`.

### 4.2 HTML Input Types

The project demonstrates several HTML5 input types.

| Input Type       | Description                               |
| ---------------- | ----------------------------------------- |
| `text`           | Single-line text input.                   |
| `email`          | Email input with browser validation.      |
| `password`       | Hides entered characters.                 |
| `radio`          | Allows selecting one option from a group. |
| `checkbox`       | Allows selecting multiple options.        |
| `file`           | Allows users to select a file.            |
| `date`           | Date picker.                              |
| `time`           | Time picker.                              |
| `week`           | Week picker.                              |
| `datetime-local` | Date and time picker.                     |
| `number`         | Numeric input.                            |
| `range`          | Slider control.                           |
| `color`          | Color picker.                             |

### 4.3 Other Form Elements

* `<select>`: Creates a dropdown menu.
* `<option>`: Defines an option inside a dropdown.
* `<textarea>`: Creates a multi-line text input.

Example:

```html
<select name="country">
    <option value="egypt">Egypt</option>
    <option value="usa">USA</option>
</select>
```

### 4.4 Important Form Attributes

| Attribute     | Description                                     |
| ------------- | ----------------------------------------------- |
| `name`        | Identifies the input when submitting form data. |
| `value`       | Defines the default or submitted value.         |
| `placeholder` | Displays a temporary hint inside an input.      |
| `required`    | Makes an input mandatory.                       |
| `min`         | Defines the minimum allowed value.              |
| `id`          | Provides a unique identifier for an element.    |

---

## ⚙️ 5. Form Functionality

### 5.1 Submit and Reset

**Reset Button:**

```html
<input type="reset" value="Reset">
```

Clears the form and restores its default values.

**Submit Button:**

```html
<input type="submit" value="Submit">
```

Submits the form data to the specified destination.

### 5.2 Using the Formaction Attribute

The `formaction` attribute allows different submit buttons to send form data to different destinations.

Example:

```html
<form method="get">

    <input type="text" name="username">

    <input type="submit"
           value="Login"
           formaction="Login.html">

    <input type="submit"
           value="Register"
           formaction="Register.html">

</form>
```

**How It Works:**

* Clicking Login redirects to `Login.html`.
* Clicking Register redirects to `Register.html`.

This demonstrates how multiple submit buttons can override the form's default destination.

### 5.3 GET vs POST

The project uses:

```html
<form method="get">
```

**GET Method:**

* Sends form data through URL parameters.
* Data appears in the browser address bar.
* Suitable for search forms and non-sensitive requests.
* Should not be used for passwords or sensitive information.

Example:

```text
?username=Ahmed&password=123
```

**POST Method:**

* Sends form data inside the HTTP request body.
* Does not normally display submitted values in the URL.
* Commonly used for registration and login forms.
* Requires HTTPS for secure transmission.


---



## 💻 6. Technologies Used

| Technology | Purpose                                            |
| ---------- | -------------------------------------------------- |
| HTML5      | Building the structure and content of the webpage. |



---

## 🧠 7. What I Learned

Through this project, I gained practical experience in:

1. Understanding the basic structure of an HTML5 document.
2. Organizing webpage content using headings and paragraphs.
3. Working with different text-formatting elements.
4. Creating internal and external hyperlinks.
5. Embedding images and managing relative file paths.
6. Creating ordered, unordered, and description lists.
7. Building HTML tables and merging cells using `rowspan`.
8. Creating forms using different HTML5 input types.
9. Connecting labels with inputs using `for` and `id`.
10. Using `fieldset` and `legend` to organize form sections.
11. Understanding the difference between GET and POST methods.
12. Using `formaction` to redirect different submit buttons to different pages.

---

## 👨‍💻 8. Developer / Contact

**Ahmed Gaber**

Computer Science Student | Passionate about Programming, Technology, and Data Analysis.

* 🔗 LinkedIn: [Ahmed Gaber](https://www.linkedin.com/in/ahmed-gaber-0424bb344)
* 📧 Email: [ahmed.kh.gaber@gmail.com](mailto:ahmed.kh.gaber@gmail.com)

---

# Thank You
