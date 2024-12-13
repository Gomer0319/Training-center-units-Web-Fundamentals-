## Styling with CSS: Basic Techniques

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Apply basic CSS properties to style text, backgrounds, and borders.
2. Understand how to style HTML elements to enhance the visual structure of web pages.

### Introduction: Adding Style to Your Web Pages

CSS (Cascading Style Sheets) is the design language used to add style and layout to web pages. With CSS, you can transform plain HTML into visually engaging content by adjusting colors, fonts, and much more. Basic CSS styling is the foundation for building visually appealing websites.

### Essential CSS Styling Properties

#### 1. **Text Styling**
Text is one of the most common elements you'll style. You can modify its appearance using CSS properties like `color`, `font-size`, and `text-align`.

- **Example:**
  ```css
  h1 {
      color: navy;
      font-size: 32px;
      text-align: center;
  }
  ```
  This styles all `<h1>` headings with a navy color, larger font size, and centered alignment.

#### 2. **Backgrounds**
CSS allows you to change the background color or add images to elements, enhancing visual appeal and providing structure to web pages.

- **Example:**
  ```css
  body {
      background-color: #f0f0f0;
  }
  ```
  This adds a light gray background to the entire webpage.

- You can also use an image as a background:
  ```css
  .hero {
      background-image: url('hero-background.jpg');
      background-size: cover;
  }
  ```

#### 3. **Borders**
Borders can be added around any HTML element to give structure or highlight specific sections. You can define the border’s width, style, and color.

- **Example:**
  ```css
  p {
      border: 2px solid black;
      padding: 10px;
  }
  ```
  This adds a solid black border around all paragraphs and provides some internal spacing with padding.

---

### Key Points
- CSS allows you to style text, backgrounds, and borders, adding visual structure to your web pages.
- Basic CSS properties form the building blocks for creating visually appealing websites.

By mastering these essential styling techniques, you can start turning basic HTML into beautifully styled content.