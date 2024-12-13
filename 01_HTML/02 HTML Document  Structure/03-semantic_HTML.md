## Semantic HTML

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Define what semantic HTML is and its significance in web development.
2. Identify semantic HTML elements and their appropriate usage.
3. Explain how semantic HTML improves accessibility and SEO.

### Introduction: Meaningful Markup

Imagine reading a book where the chapters are not clearly marked, and paragraphs are randomly scattered. It would be confusing, right? **Semantic HTML** is like a well-organized book; it uses meaningful tags to describe the content, making it easier for browsers and users to understand the structure and purpose of the information on a webpage.

### What is Semantic HTML?

**Semantic HTML** refers to using HTML tags that convey meaning about the content enclosed within them. Instead of using generic tags like `<div>` or `<span>`, semantic tags provide more context and clarity about the role of the content on the page. This practice enhances readability for both humans and machines.

### Common Semantic HTML Elements

Here are some key semantic HTML elements and their purposes:

#### 1. **Header (`<header>`)**
- Represents the introductory content or navigational links for a section or page.
  
  **Example:**
  ```html
  <header>
      <h1>Website Title</h1>
      <nav>
          <ul>
              <li><a href="#home">Home</a></li>
              <li><a href="#about">About</a></li>
          </ul>
      </nav>
  </header>
  ```

#### 2. **Navigation (`<nav>`)**
- Defines a set of navigation links, usually for navigating through different sections of the website.
  
  **Example:**
  ```html
  <nav>
      <ul>
          <li><a href="#services">Services</a></li>
          <li><a href="#contact">Contact</a></li>
      </ul>
  </nav>
  ```

#### 3. **Main (`<main>`)**
- Represents the dominant content of the `<body>` and should be unique to the document.
  
  **Example:**
  ```html
  <main>
      <h2>Main Content</h2>
      <p>This is the primary content of the webpage.</p>
  </main>
  ```

#### 4. **Section (`<section>`)**
- Represents a thematic grouping of content, typically with a heading.
  
  **Example:**
  ```html
  <section>
      <h2>About Us</h2>
      <p>Information about the company.</p>
  </section>
  ```

#### 5. **Article (`<article>`)**
- Represents a self-contained piece of content that can be distributed independently, such as a blog post or news article.
  
  **Example:**
  ```html
  <article>
      <h2>Blog Post Title</h2>
      <p>This is the content of the blog post.</p>
  </article>
  ```

#### 6. **Footer (`<footer>`)**
- Contains footer information for a section or the entire page, such as copyright and contact details.
  
  **Example:**
  ```html
  <footer>
      <p>&copy; 2024 My Website. All rights reserved.</p>
  </footer>
  ```

#### 7. **Aside (`<aside>`)**
- Represents content that is related to the main content but can stand alone, like sidebars or pull quotes.
  
  **Example:**
  ```html
  <aside>
      <h2>Related Information</h2>
      <p>This is additional content related to the main topic.</p>
  </aside>
  ```

### Benefits of Semantic HTML

1. **Improved Accessibility**: Semantic HTML helps screen readers and assistive technologies understand the structure and purpose of content, making websites more accessible to users with disabilities.
  
2. **Enhanced SEO**: Search engines use semantic tags to better understand the content of a webpage, which can lead to improved search rankings.

3. **Better Maintainability**: Using meaningful tags makes the code easier to read and maintain for developers, improving collaboration and reducing errors.

---

### Key Points
- Semantic HTML uses meaningful tags that describe the content, improving readability and accessibility.
- Key semantic elements include `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`, and `<aside>`.
- Adopting semantic HTML practices enhances user experience, accessibility, and search engine optimization.