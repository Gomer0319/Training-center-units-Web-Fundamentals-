## Build Your Personal Profile: Showcase Your Skills!

### Trainee Goal
By completing this assignment, trainees will:
1. Create a simple personal profile webpage using basic HTML elements.
2. Learn how to structure a webpage with semantic tags.
3. Include images to enhance their profile representation.
4. Organize information effectively within their profile.

### Duration
30 minutes to 1 hour

### Difficulty
Beginner

### Instructions
Your task is to create a simple personal profile webpage that showcases who you are and the technologies you've learned. Follow these steps:

1. **Create a new HTML file** named `first_last_profile.html`, replacing `first` and `last` with your actual first and last name (e.g., `john_doe_profile.html`).
2. **Structure your webpage** using semantic HTML tags, such as `<header>`, `<main>`, `<section>`, and `<footer>`.
3. **Include the following sections**:
   - **Header**: Your name and a brief tagline.
   - **About Me**: A short paragraph introducing yourself.
   - **Skills**: A section highlighting your skills in technology.
   - **Interests**: A section that reflects your personal interests or hobbies.
   - **Images**: Download and attach images representing the technologies you know. Ensure they are relevant and appropriately named.
4. Use semantic HTML elements to organize your content, considering how lists might help present your skills and interests clearly.
5. Save your HTML file and ensure it is properly formatted and indented.
6. Submit your `first_last_profile.html` file via the designated submission portal.

### Bonus Task: Visual Appeal
For extra points:
- Consider how you might enhance the visual appearance of your profile page using HTML. Think about structure and layout, even if you won't be using CSS yet.

### Criteria for Success
Your submission will be evaluated based on:
- **Effective use of semantic tags**: Proper use of tags to structure the page logically.
- **Content organization**: Clear organization of information into appropriate sections.
- **Information presentation**: Thoughtful use of HTML elements to convey your skills and interests.
- **Image inclusion**: Correctly attached images representing the technologies learned, ensuring they are well integrated into the profile.
- **Proper formatting**: Ensure proper indentation and cleanliness of code.

---

### Solution

Here’s an example solution for your reference. You can modify the content as per your personal information:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>John Doe's Personal Profile</title>
</head>
<body>
  <header>
    <h1>John Doe</h1>
    <p>Aspiring Web Developer</p>
  </header>
  
  <main>
    <section>
      <h2>About Me</h2>
      <p>Hello! I am a passionate web developer with a love for creating interactive and user-friendly web applications.</p>
    </section>
    
    <section>
      <h2>Skills</h2>
      <p>Here are some of the technologies I am familiar with:</p>
      <ol>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
      </ol>
    </section>
    
    <section>
      <h2>Interests</h2>
      <p>Some of my personal interests include:</p>
      <ul>
        <li>Coding</li>
        <li>Reading</li>
        <li>Traveling</li>
      </ul>
    </section>
    
    <section>
      <h2>Technologies</h2>
      <h3>HTML</h3>
      <img src="path/to/your/html-image.png" alt="HTML Logo" />
      <h3>CSS</h3>
      <img src="path/to/your/css-image.png" alt="CSS Logo" />
      <h3>JavaScript</h3>
      <img src="path/to/your/js-image.png" alt="JavaScript Logo" />
    </section>
  </main>
  
  <footer>
    <p>Contact me at johndoe@example.com</p>
  </footer>
</body>
</html>
```
