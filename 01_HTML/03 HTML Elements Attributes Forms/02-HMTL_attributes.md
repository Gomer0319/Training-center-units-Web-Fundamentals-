## HTML Attributes

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand what HTML attributes are and their role in modifying HTML elements.
2. Identify common HTML attributes and their uses.
3. Apply attributes to elements to add additional functionality or styling.

### Introduction: Adding Details to HTML Elements

Think of HTML attributes like labels or settings for elements, providing extra information or instructions on how those elements should behave. Just as a car’s features like color, model, or engine type provide more detail about the vehicle, HTML attributes do the same for elements, specifying properties such as width, height, or behavior.

### Key Concepts

#### 1. **What are HTML Attributes?**
- HTML attributes provide additional information about an HTML element, typically included inside the opening tag of the element.
- Each attribute consists of a **name** and a **value**. The value is wrapped in quotation marks.

  **Example:**
  ```html
  <a href="https://www.example.com">Visit Example Website</a>
  ```
  In this example:
  - `href` is the attribute name.
  - `"https://www.example.com"` is the attribute value.
  - Together, they define the destination of the link.

#### 2. **Common HTML Attributes**

- **`href`**: Used with `<a>` (anchor) tags to specify the URL of a link.
  ```html
  <a href="https://www.example.com">Visit Example Website</a>
  ```

- **`src`**: Used with `<img>` or `<iframe>` tags to specify the source URL of an image or embedded content.
  ```html
  <img src="image.jpg" alt="An image description">
  ```

- **`alt`**: Provides alternative text for images, used for accessibility.
  ```html
  <img src="image.jpg" alt="A description of the image">
  ```

- **`id`**: Assigns a unique identifier to an element for CSS styling or JavaScript manipulation.
  ```html
  <div id="header">This is the header section</div>
  ```

- **`class`**: Assigns one or more class names to an element, used to group elements for styling or interaction.
  ```html
  <p class="intro">This is an introductory paragraph.</p>
  ```

- **`style`**: Adds inline CSS to an element.
  ```html
  <p style="color: blue;">This text is blue.</p>
  ```

- **`title`**: Displays additional information as a tooltip when hovering over an element.
  ```html
  <a href="#" title="More information">Hover over me</a>
  ```

#### 3. **Using Multiple Attributes**
- An HTML element can have more than one attribute. Each attribute is separated by a space within the opening tag.
  
  **Example:**
  ```html
  <img src="image.jpg" alt="Sample Image" width="300" height="200">
  ```
  Here, the image element has three attributes: `src`, `alt`, `width`, and `height`.

#### 4. **Global Attributes**
- Some attributes can be applied to any HTML element, known as **global attributes**. Common global attributes include:
  - **`id`**: Unique identifier.
  - **`class`**: Class name for CSS.
  - **`style`**: Inline CSS for styling.
  - **`title`**: Tooltip text.

  **Example:**
  ```html
  <div id="footer" class="main-footer" style="background-color: lightgray;" title="This is the footer section.">
    Footer Content
  </div>
  ```

---

### Key Points
- HTML attributes provide extra details or instructions about elements.
- Common attributes include `href`, `src`, `alt`, `id`, and `class`.
- Multiple attributes can be used in a single element, each separated by spaces.
- Global attributes, like `id`, `class`, and `style`, can be applied to any element for more flexibility in design and interactivity.