## Level Up Your HTML: From Divs to Meaning!

### Trainee Goal
By completing this assignment, trainees will:
- Understand how to improve code readability by using semantic HTML tags.
- Learn how to replace generic `<div>` tags with appropriate semantic tags.
- Apply correct indentation for cleaner and more professional HTML structure, in line with industry best practices.

### Duration
30 minutes to 1 hour

### Difficulty
Intermediate

### Instructions
You are provided with an unindented HTML file (below) that contains several `<div>` tags and inconsistent formatting. Your task is to:
1. **Replace** all unnecessary `<div>` tags with correct **semantic HTML tags** such as `<header>`, `<section>`, `<article>`, `<footer>`, etc.
2. **Indent the HTML properly** for improved readability and structure based on the relationships between parent and child elements.
3. Ensure that you **use appropriate header tags** (e.g., `<h1>`, `<h2>`, `<h3>`) to structure content clearly.
4. Convert any unordered lists into **ordered lists** using `<ol>` and `<li>` for content that follows a logical sequence. Separate the lists into distinct sections if applicable.
5. Submit your corrected HTML file via the submission portal provided.

### HTML File to Correct:

```html
<html>
<head>
  <title>My Website</title>
</head>
<body>
<div class="header">
<div class="logo">My Website</div>
<div class="nav">
<div class="link"><a href="#">Home</a></div>
<div class="link"><a href="#">About</a></div>
<div class="link"><a href="#">Contact</a></div>
</div>
</div>
<div class="main-content">
<div class="section">
<div class="article">
<div class="title">The Importance of Semantic HTML</div>
<div class="body">
<p>Semantic HTML improves SEO and accessibility...</p>
<div class="list">
<ul>
<li>Better SEO</li>
<li>Improved accessibility</li>
<li>Clearer structure</li>
</ul>
</div>
</div>
</div>
</div>
<div class="footer">
<div class="contact-info">
<p>Email us at info@example.com</p>
</div>
</div>
</body>
</html>
```

### Bonus Task: The SEO Boost Challenge
For extra points:
- Make sure the hierarchy of header tags (`<h1>`, `<h2>`, `<h3>`, etc.) follows a logical structure that improves both readability and SEO.

### Criteria for Success
Your submission will be evaluated based on:
- **Effective use of semantic tags**: Replace every unnecessary `<div>` tag with an appropriate semantic HTML element.
- **Proper indentation**: Ensure that all nested elements are indented according to their parent-child relationships.
- **Logical use of ordered lists**: Convert unordered lists (`<ul>`, `<li>`) into ordered lists (`<ol>`, `<li>`) where sequential content is necessary and organize them into distinct sections.
- **Content hierarchy**: Use header tags logically to create a meaningful structure for the page’s content.
- **Bonus points**: Extra credit for correctly using and structuring header tags to improve SEO.

---

### Solution

Here is one possible solution to the assignment with proper semantic tags, indentation, and ordered lists applied:

```html
<html>
<head>
  <title>My Website</title>
</head>
<body>
  <header>
    <div class="logo">My Website</div>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>
  
  <main>
    <section>
      <article>
        <h1>The Importance of Semantic HTML</h1>
        <div class="body">
          <p>Semantic HTML improves SEO and accessibility...</p>
        </div>
      </article>
    </section>
    
    <section>
      <h2>Benefits of Semantic HTML</h2>
      <ol>
        <li>Better SEO</li>
        <li>Improved accessibility</li>
        <li>Clearer structure</li>
      </ol>
    </section>
  </main>
  
  <footer>
    <section class="contact-info">
      <p>Email us at info@example.com</p>
    </section>
  </footer>
</body>
</html>
```

---

This solution demonstrates:
- **Semantic tags**: Unnecessary `<div>` tags were replaced with semantic elements like `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, and `<footer>`.
- **Logical sectioning**: The list of benefits was separated into a distinct section with proper heading structure.
- **Ordered list**: The unordered list was converted into an ordered list, showing sequential points.