## Enhance Your Portfolio: Apply Basic Styling

### Trainee Goal
By completing this assignment, trainees will:
1. Apply basic CSS to enhance their portfolio.
2. Adjust colors, widths, heights, and fonts using pixel values for precise control.
3. Understand how basic styling affects the structure of an HTML page.

### Duration
45 minutes to 1 hour

### Difficulty
Intermediate

### Instructions
You will add basic styling to your portfolio using CSS, following these steps:

1. Open your `first_last_profile2.html` file (example: `juan_dela_cruz_profile2.html`).
2. Create a `styles.css` file and link it in your HTML.
3. Apply the following:
   - Set a background color for the page.
   - Modify font colors, sizes, and headings using pixel values (only use `px` for sizing).
   - Adjust image widths and heights using pixels.
   - Use pixel values for padding and margins to ensure consistent spacing.

4. **Submission**: Place the updated HTML and CSS files, along with any local assets, into a folder. Compress the folder and rename it to `first_last_profile2_css.zip` before submitting.

### Bonus Task: Hover Effects on Submit Button
For extra points:
- Add a hover effect to the "Submit" button in the Contact Us form.

### Criteria for Success
Evaluation will be based on:
- Proper use of basic CSS with pixel-based sizes for color, font styles, and spacing.
- Clean code structure with proper formatting.
- **Bonus**: Effective hover effects on the submit button.

---

### Solution

**HTML (first_last_profile2.html):**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>John Doe Portfolio</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <h1>John Doe</h1>
    <p>Web Developer</p>
  </header>

  <section>
    <h2>About Me</h2>
    <p>Passionate web developer skilled in HTML, CSS, and JavaScript.</p>
  </section>

  <section>
    <h2>Technologies I Use</h2>
    <ul>
      <li><img src="html_logo.png" alt="HTML" width="100px"></li>
      <li><img src="css_logo.png" alt="CSS" width="100px"></li>
      <li><img src="js_logo.png" alt="JS" width="100px"></li>
    </ul>
  </section>

  <section>
    <h2>Contact Us</h2>
    <form>
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>

      <label for="name">Name:</label>
      <input type="text" id="name" name="name">

      <label for="message">Message:</label>
      <textarea id="message" name="message"></textarea>

      <button type="submit">Submit</button>
    </form>
  </section>
</body>
</html>
```

**CSS (styles.css):**

```css
body {
  background-color: #f4f4f4;
  font-family: Arial, sans-serif;
}

header {
  text-align: center;
  background-color: #333;
  color: white;
  padding: 20px;
}

h1 {
  font-size: 40px;
}

ul {
  padding: 0;
}

ul li {
  display: inline-block;
  margin-right: 15px;
}

form {
  padding: 10px;
}

input, textarea {
  margin-bottom: 10px;
  padding: 10px;
  width: 250px;
}

button {
  background-color: #333;
  color: white;
  padding: 10px 20px;
  border: none;
}

button:hover {
  background-color: #555;
}
```
