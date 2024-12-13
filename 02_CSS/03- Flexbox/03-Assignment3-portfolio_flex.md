### Assignment: Flex Your Portfolio Design

#### Trainee Goal:
1. Implement `flex` display and its properties to enhance the layout of your portfolio.
2. Organize and align elements more efficiently using `flex` containers and items.
3. Apply flexbox properties to create a clean and organized visual layout for your portfolio.

#### Duration:
1 - 2 hours

#### Difficulty:
Intermediate

#### Instructions:
1. Open your existing **first_last_profile_css_updated.zip** file and locate your **first_last_profile2.html** and **styles.css** files.
2. In your **styles.css** file, update the layout using `flex` display and properties:
   - Set appropriate containers to `display: flex` to control the alignment and distribution of child elements.
   - Utilize flex properties such as `justify-content`, `align-items`, and `flex-direction` to organize and align content effectively.
   - Improve the structure and flow of your portfolio by leveraging flexbox for layout arrangement.
3. **Submission**: Once you are satisfied with your updates, compress the folder containing your HTML and CSS files, and rename it to **first_last_profile_flex.zip** before submitting.

#### Bonus Task:
- Use `flex-wrap` to ensure content adjusts and wraps within the flex container, particularly for larger sets of images or text blocks.

#### Criteria for Success:
- **Flex Usage**: Clear and proper use of `flex` display properties to create an improved layout.
- **Alignment and Spacing**: Proper organization of elements using flex properties like `justify-content`, `align-items`, and `flex-direction`.
- **Layout Structure**: Cohesive and visually pleasing structure using flexbox.

---

### Solution:

#### HTML (first_last_profile2.html):

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>John Doe</h1>
        <nav>
            <ul>
                <li><a href="#about">About Me</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#contact">Contact Me</a></li>
            </ul>
        </nav>
    </header>

    <section id="about">
        <h2>About Me</h2>
        <p>I am a web developer passionate about learning new technologies.</p>
    </section>

    <section id="skills">
        <h2>Skills</h2>
        <div class="skills-container">
            <div class="skill">
                <img src="path/to/html_image.jpg" alt="HTML">
                <p>HTML</p>
            </div>
            <div class="skill">
                <img src="path/to/css_image.jpg" alt="CSS">
                <p>CSS</p>
            </div>
            <div class="skill">
                <img src="path/to/js_image.jpg" alt="JavaScript">
                <p>JavaScript</p>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Me</h2>
        <form>
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required><br>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required><br>
            
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea><br>
            
            <button type="submit">Submit</button>
        </form>
    </section>

</body>
</html>
```

---

#### CSS (styles.css):

```css
/* Global Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: white;
    padding: 10px;
    text-align: center;
}

header nav ul {
    list-style: none;
    padding: 0;
}

header nav ul li {
    display: inline;
    margin-right: 15px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
}

/* Flexbox Layout */
.skills-container {
    display: flex;
    justify-content: space-around;
    align-items: center;
    margin: 20px 0;
}

.skill {
    text-align: center;
}

.skill img {
    width: 100px;
    height: 100px;
}

/* Contact Form */
form {
    display: flex;
    flex-direction: column;
    width: 50%;
    margin: 0 auto;
}

label, input, textarea, button {
    margin-bottom: 10px;
}
```