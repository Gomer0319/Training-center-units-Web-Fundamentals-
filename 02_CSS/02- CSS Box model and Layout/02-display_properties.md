## Basic Display Properties in CSS

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand the key CSS display properties and their roles in element positioning.
2. Differentiate between block, inline, and inline-block elements.
3. Apply display properties to control the layout and behavior of HTML elements.

### Introduction: How Display Properties Shape Web Layouts

CSS **display properties** define how HTML elements are displayed on a webpage. These properties control how an element behaves in the document’s layout—whether it appears in a line, takes up the full width of a page, or remains hidden. Understanding display properties is critical for managing the structure and appearance of web pages.

### Key Display Values

#### 1. **Block**
Elements with a `display: block` property take up the full width of their container and start on a new line. Common examples of block elements include `<div>`, `<p>`, and `<h1>`.

- **Example:**
  ```css
  div {
      display: block;
  }
  ```
  This makes the `<div>` element a block-level element, taking up the entire width of the container.

- Block elements:
  - Occupy the full width available.
  - Always start on a new line.

#### 2. **Inline**
Elements with a `display: inline` property do not start on a new line and only take up as much width as necessary. Common inline elements include `<span>`, `<a>`, and `<img>`.

- **Example:**
  ```css
  span {
      display: inline;
  }
  ```
  This makes the `<span>` element inline, meaning it can exist within a block of text without forcing a line break.

- Inline elements:
  - Take up only as much width as the content.
  - Do not start on a new line.

#### 3. **Inline-block**
The `display: inline-block` property combines the characteristics of both inline and block elements. Inline-block elements remain inline with other elements but allow for setting width and height, unlike purely inline elements.

- **Example:**
  ```css
  img {
      display: inline-block;
      width: 150px;
      height: 100px;
  }
  ```
  This allows the `<img>` element to behave like an inline element while still allowing control over its size.

- Inline-block elements:
  - Do not start on a new line.
  - Allow width and height adjustments.

#### 4. **None**
The `display: none` property hides an element completely, removing it from the document flow. It will not take up any space on the page, but it remains in the HTML code.

- **Example:**
  ```css
  .hidden {
      display: none;
  }
  ```
  This makes any element with the `hidden` class completely invisible on the page.

### Using Display Properties in Layouts

Display properties are often used to manage layout structure. For example, making a parent `<div>` block-level and its child elements inline-block allows for creating flexible layouts without breaking the flow of content.

- **Example Layout:**
  ```css
  .container {
      display: block;
  }

  .box {
      display: inline-block;
      width: 100px;
      height: 100px;
      background-color: lightblue;
      margin: 10px;
  }
  ```

  ```html
  <div class="container">
      <div class="box"></div>
      <div class="box"></div>
      <div class="box"></div>
  </div>
  ```
  In this example, each `.box` element is displayed inline within the container but can have individual widths and heights, creating a simple grid-like layout.

---

### Key Points
- **Block** elements take up the entire width and start on a new line, while **inline** elements stay within the content flow.
- **Inline-block** elements combine features of both, remaining inline while allowing for width and height adjustments.
- **Display: none** hides an element from the layout entirely, making it invisible but still present in the code.

Understanding and using the display property correctly allows you to control how elements are arranged and displayed on the page, offering flexibility in structuring web content.