# HTML Tags 1

## HTML Structure

An HTML file has the `.html` extension and begins with the document type declaration:

```html
<!DOCTYPE html>
```

The entire content is wrapped in the `<html>` tag:

```html
<html>
  <!-- Content goes here -->
</html>
```

### Main Sections of an HTML Document

1. **Head (`<head>`)** – Contains metadata and links to resources like stylesheets and scripts.

   - `<title>` – Sets the title shown in the browser tab.
   - `<meta>` tags – Provide metadata for search engines (SEO), e.g.,
     - `name` – Specifies the type of metadata (e.g., "description", "keywords", "author").
     - `content` – The actual value for the metadata.
   - Links to external styles (`<link>`) and scripts (`<script>`).

2. **Body (`<body>`)** – Contains the visible content of the webpage.

### Viewing an HTML Page

After saving the file with a `.html` extension, open it in a browser to view the rendered content.

> **SEO (Search Engine Optimization)**: Practices that enhance a website's visibility on search engines.

---

## Header Tags: `<h1>`, `<h2>`, ..., `<h6>`

Header tags structure content hierarchically, improving content organization and SEO.

- **`<h1>`** – First-level header (most important).
- **`<h2>`** – Second-level header.
- **`<h3>`** – Third-level header.
- **`<h4>`** – Fourth-level header.
- **`<h5>`** – Fifth-level header.
- **`<h6>`** – Sixth-level header (least important).

### Example:

```html
<h1>Header 1</h1>
<h2>Header 2</h2>
<h3>Header 3</h3>
<h4>Header 4</h4>
<h5>Header 5</h5>
<h6>Header 6</h6>
```

This structure organizes content and is useful for both users and search engines.

---

## `<p>` Tag

The `<p>` tag is used for paragraphs.

```html
<p>This is a paragraph.</p>
```

---

## `<a>` Tag

The `<a>` tag creates hyperlinks.

```html
<a href="https://www.example.com">This is a link</a>
```

- `href` – Specifies the target URL (absolute or relative).
- The text between the opening and closing `<a>` tags is the clickable link.
- `target` attribute options:
  - `_blank` – Opens in a new tab.
  - `_self` – Opens in the same tab (default).
  - `_parent` – Opens in the parent frame.
  - `_top` – Opens in the full window.

---

## `<img>` Tag

The `<img>` tag embeds images in a webpage.

```html
<img src="image.jpg" alt="Description of the image" />
```

- `src` – Specifies the image path.
- `alt` – Provides alternative text if the image can't load and improves accessibility.
- `width` and `height` – Set the image dimensions.
- `title` – Provides additional info when hovered.
- The `<img>` tag is self-closing and doesn’t require a closing tag.
- The `alt` attribute is crucial for SEO and accessibility.

---

## Combining `<a>` and `<img>` Tags

You can make an image clickable by combining the `<a>` and `<img>` tags.

```html
<a href="https://www.example.com">
  <img src="image.jpg" alt="Description of the image" />
</a>
```

- Clicking on the image will redirect the user to the specified URL.
- Useful for image-based navigation or linking to a larger image.

# HTML Tags 2

## `<div>` and `<span>` Tags

### `<div>` (Block Container)

- A **block-level** container used for grouping multiple elements.
- Commonly used for styling with CSS and scripting with JavaScript.

### `<span>` (Inline Container)

- An **inline** container for styling or manipulating a small part of the text.
- Often used for highlighting text or applying actions to inline elements.

#### Example:

```html
<div class="container">
  <h1>Header</h1>
  <p>
    This is a paragraph with <span class="highlight">highlighted text</span>.
  </p>
</div>
```

---

### Inline vs. Block Elements

| Type                      | Description                                                                                       |
| ------------------------- | ------------------------------------------------------------------------------------------------- |
| **Block Elements**        | Take up the full width of their parent container (e.g., `<div>`, `<p>`, `<h1>`-`<h6>`)            |
| **Inline Elements**       | Take up only as much width as necessary (e.g., `<span>`, `<a>`, `<img>`)                          |
| **Inline-Block Elements** | Behave like inline elements but allow setting width/height (e.g., `<img>`, `<input>`, `<button>`) |

---

## Semantic Tags

### Common Semantic Elements

| Tag            | Purpose                                            |
| -------------- | -------------------------------------------------- |
| `<header>`     | Contains the logo and title.                       |
| `<nav>`        | Holds navigation links.                            |
| `<section>`    | Groups related content.                            |
| `<footer>`     | Contains copyright and contact info.               |
| `<article>`    | Represents independent content (e.g., blog posts). |
| `<aside>`      | Sidebar content related to the main content.       |
| `<figure>`     | Groups media content (images, videos, etc.).       |
| `<figcaption>` | Provides a caption for a `<figure>`.               |

Semantic tags **improve SEO** and **accessibility**, making the document structure more meaningful.

### Example:

```html
<header>
  <img src="logo.png" alt="Logo" />
  <h1>Website Title</h1>
  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<main>
  <section id="home">
    <h2>Welcome to Our Website</h2>
    <p>This is the home section.</p>
  </section>
  <section id="about">
    <h2>About Us</h2>
    <p>This is the about section.</p>
  </section>
  <section id="contact">
    <h2>Contact Us</h2>
    <p>This is the contact section.</p>
  </section>
</main>

<footer>
  <p>&copy; 2023 Your Website. All rights reserved.</p>
</footer>
```

### **Advantages of Semantic Tags:**

✔ Better for **SEO** (search engines understand the structure better).  
✔ Improves **accessibility** (helps screen readers and assistive devices).  
✔ Enhances **code readability** and organization.

---

## `<table>` Tag

The `<table>` tag is used to create tables.

### Table Structure:

- **`<thead>`** – Table header section
- **`<tbody>`** – Table body section
- **`<tr>`** – Defines a table row
- **`<th>`** – Table header cell (bold and centered by default)
- **`<td>`** – Table data cell (regular text)

### Example:

```html
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Age</th>
      <th>Gender</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Mohammad</td>
      <td>24</td>
      <td>Male</td>
    </tr>
    <tr>
      <td>Heba</td>
      <td>23</td>
      <td>Female</td>
    </tr>
  </tbody>
</table>
```

# HTML Forms

## Text and Password Inputs

Text and password fields allow users to enter information into a form.

- `<input>` is used to create form input fields.
- `type="text"` – Creates a **single-line text** input.
- `type="password"` – Creates a **password** input (characters are hidden).
- `placeholder` – Provides a hint to the user.
- `name` – Identifies the field when submitting the form (for backend processing).

### **Labels**

The `<label>` tag is used to associate a text description with an input field.

- The `for` attribute in `<label>` should match the `id` of the input field for accessibility.

#### **Example:**

```html
<form>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" placeholder="Enter your name" />
  <br />
  <label for="password">Password:</label>
  <input
    type="password"
    id="password"
    name="password"
    placeholder="Enter your password"
  />
</form>
```

---

## Checkbox Input

Checkboxes allow users to **select multiple** options.

- Uses `<input type="checkbox">`.
- The `name` attribute groups checkboxes.
- The `value` attribute specifies the value sent to the server.

#### **Example:**

```html
<form>
  <input type="checkbox" name="food" id="pizza" value="pizza" />
  <label for="pizza">Pizza</label>

  <input type="checkbox" name="food" id="burger" value="burger" />
  <label for="burger">Burger</label>

  <input type="checkbox" name="food" id="pasta" value="pasta" />
  <label for="pasta">Pasta</label>
</form>
```

---

## Radio Buttons

Radio buttons allow users to **select one** option from a list.

- Uses `<input type="radio">`.
- All related options must have the **same `name`**.
- The `value` specifies what is sent to the server.

#### **Example:**

```html
<form>
  <p>Gender:</p>
  <input type="radio" name="gender" id="male" value="male" />
  <label for="male">Male</label>

  <input type="radio" name="gender" id="female" value="female" />
  <label for="female">Female</label>
</form>
```

---

## Dropdown (`<select>` tag)

Dropdowns allow users to **select one option** from a list.

- Uses `<select>` with `<option>` elements inside.
- The `value` attribute is what gets sent to the server.

#### **Example:**

```html
<form>
  <label for="country">Select your country:</label>
  <select name="country" id="country">
    <option value="jordan">Jordan</option>
    <option value="uk">UK</option>
    <option value="canada">Canada</option>
    <option value="australia">Australia</option>
    <option value="uae">UAE</option>
  </select>
</form>
```

---

## **Textarea (Multi-line Input)**

The `<textarea>` tag allows users to enter **multi-line text**.

- `rows` and `cols` define size (optional).
- The `name` attribute is required to capture the input when submitting.

#### **Example:**

```html
<form>
  <label for="message">Message:</label>
  <textarea id="message" name="message" rows="4" cols="50"></textarea>
</form>
```

---

## **Form Submission**

A **submit button** sends the form data to the server.

- Uses `<input type="submit">` or `<button type="submit">`.
- The `action` attribute defines **where** to send the data.
- The `method` specifies **how** to send the data:
  - **GET** – Appends form data to the URL (not secure).
  - **POST** – Sends data in the request body (more secure).

#### **Example:**

```html
<form action="submit_form.php" method="post">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required />
  <br />

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required />
  <br />

  <input type="submit" value="Submit" />
  or
  <button type="submit">Submit</button>
</form>
```

---

## **Summary of Form Elements**

| Tag                       | Purpose                                |
| ------------------------- | -------------------------------------- |
| `<input type="text">`     | Single-line text input                 |
| `<input type="password">` | Password input (hidden characters)     |
| `<input type="checkbox">` | Allows multiple selections             |
| `<input type="radio">`    | Allows only one selection from a group |
| `<select>`                | Creates a dropdown list                |
| `<textarea>`              | Multi-line text input                  |
| `<input type="submit">`   | Submit button                          |
