## Targeting Elements: CSS Selectors

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand the role of CSS selectors in targeting HTML elements.
2. Identify and use basic CSS selectors (type, class, ID).
3. Apply more specific selectors (attribute, descendant, pseudo-classes) to control styling with precision.

### Introduction: Choosing What to Style with CSS Selectors

In CSS, **selectors** determine which HTML elements get styled. Without selectors, CSS wouldn’t know which parts of the page you want to apply styles to. CSS selectors are incredibly powerful because they allow you to be as broad or specific as you need, whether you're styling every paragraph on a page or targeting a single element.

### Key Types of CSS Selectors

#### 1. **Type Selector**
The most basic selector targets all elements of a specific HTML tag. For example, a type selector for paragraphs will style every `<p>` tag on the page.

- **Example:**
  ```css
  p {
      color: blue;
  }
  ```
  This rule will make all paragraph text blue.

#### 2. **Class Selector**
A class selector targets elements that have a specific class attribute. This is useful when you want to apply styles to multiple elements, but not all elements of the same type.

- **Example:**
  ```css
  .button {
      background-color: green;
      color: white;
  }
  ```
  The class `.button` can be used on any element, like a `<div>` or `<a>`, and will apply the styles to those elements.

- **HTML Usage:**
  ```html
  <a class="button">Click Me</a>
  ```

#### 3. **ID Selector**
The ID selector is even more specific and targets a single element with a unique `id`. IDs should only be used once per page.

- **Example:**
  ```css
  #header {
      background-color: lightgray;
      padding: 10px;
  }
  ```

- **HTML Usage:**
  ```html
  <div id="header">Welcome to My Website</div>
  ```
  
---

### Key Points
- CSS selectors are essential for applying styles to the right elements on a webpage.
- **Type, class, and ID selectors** allow basic and flexible targeting of elements.
- More advanced selectors, like **attribute**, **descendant**, and **pseudo-classes**, offer greater control for specific styling needs.

Selectors let you craft the look and feel of your website by targeting exactly the elements you want to style. Understanding and mastering them will enable you to write cleaner, more efficient CSS for any project.