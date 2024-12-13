## Introduction to CSS: Styling the Web

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand the role of CSS in web development and its importance in styling HTML pages.
2. Identify the different ways to apply CSS to an HTML document.
3. Connect CSS to an HTML document using inline, internal, and external methods.

### Bringing Style to Web Pages

CSS (Cascading Style Sheets) is the language used to style and layout web pages. While HTML is responsible for the structure and content of a webpage, CSS defines how that content looks—its colors, fonts, spacing, and layout. Think of CSS as the "design" layer of a website. It allows you to create visually appealing pages by controlling the presentation of HTML elements.

### What CSS Does
CSS gives you control over the **visual appearance** of your website by allowing you to:
- **Change Colors**: Adjust text, background, and border colors.
- **Modify Layout**: Set the position of elements, create spacing between sections, and organize content.
- **Style Text**: Change fonts, text size, alignment, and decoration (like underlining or bolding).
- **Adjust Sizes**: Set width, height, and proportions of elements.
- **Responsive Design**: Ensure that web pages look good on different devices (desktop, tablet, mobile).

**Example:**
With HTML alone, a heading looks like this:
```html
<h1>Hello World</h1>
```

Using CSS, you can style it:
```css
h1 {
    color: blue;
    font-family: Arial, sans-serif;
    text-align: center;
}
```
Now, the heading "Hello World" is blue, centered, and uses the Arial font.

### How to Connect CSS to HTML

There are three main ways to connect CSS to an HTML document:

1. **Inline CSS**:
   - Applied directly inside the HTML element using the `style` attribute.
   
   **Example:**
   ```html
   <p style="color: red;">This is red text.</p>
   ```

2. **Internal CSS**:
   - Defined within the `<style>` tag in the `<head>` section of the HTML document. This method applies styles to the whole page.
   
   **Example:**
   ```html
   <head>
       <style>
           p {
               color: green;
               font-size: 18px;
           }
       </style>
   </head>
   ```

3. **External CSS** (Recommended):
   - A separate CSS file is linked to the HTML document using the `<link>` tag. This method is ideal for maintaining cleaner code and reusing styles across multiple pages.
   
   **Example:**
   HTML file:
   ```html
   <head>
       <link rel="stylesheet" href="styles.css">
   </head>
   ```

   CSS file (`styles.css`):
   ```css
   p {
       color: purple;
       font-size: 20px;
   }
   ```

This method keeps the styling separate from the HTML structure, making your code more organized and maintainable.

---

### Key Points
- CSS is used to style and format web pages, making them visually engaging.
- You can apply CSS directly in the HTML (inline), within the HTML document (internal), or in a separate file (external) for better code organization.