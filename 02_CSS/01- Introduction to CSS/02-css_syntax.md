## CSS Syntax

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand the basic structure of CSS rules.
2. Identify the components of a CSS rule: selectors, properties, and values.
3. Write valid CSS syntax to style HTML elements.

### Structuring Style: CSS Syntax

Just like sentences follow grammar rules in a language, CSS has a specific syntax that ensures styles are applied correctly to web pages. In CSS, we define **rules** that tell the browser how to style specific HTML elements. Understanding the basic syntax of CSS is key to effectively designing web pages.

### Key Components of CSS Syntax

CSS rules consist of two main parts: the **selector** and the **declaration block**. Let’s break this down:

#### 1. **Selector**
The selector specifies which HTML element(s) you want to style. It "selects" the element by name, class, ID, or attribute.

- Example of a selector for all paragraphs:
  ```css
  p {
      /* Declarations go here */
  }
  ```

#### 2. **Declaration Block**
The declaration block contains the **property** and **value** pairs, which define what styles to apply to the selected element. Declarations are enclosed in curly braces `{ }` and separated by a semicolon `;`.

- **Property**: The characteristic of the element you want to change (e.g., color, font-size, margin).
- **Value**: The specific setting for that property (e.g., `red` for color, `20px` for font-size).

**Example:**
```css
p {
    color: red;
    font-size: 16px;
}
```
In this example:
- The selector `p` targets all paragraph elements.
- The declarations set the paragraph text color to red and the font size to 16 pixels.

#### 3. **Multiple Declarations**
You can include multiple declarations inside one declaration block by separating them with semicolons.

**Example:**
```css
h1 {
    color: blue;
    text-align: center;
    margin-top: 20px;
}
```
Here, the `h1` selector is styled with three properties: blue text color, centered alignment, and 20 pixels of space at the top.

---

### Key Points
- CSS rules consist of a **selector** and a **declaration block**.
- The declaration block contains **properties** (like color, margin) and their associated **values** (like red, 20px).
- Multiple properties can be applied to a single selector by listing them inside the declaration block, separated by semicolons.