## HTML Elements

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand what HTML elements are and how they structure web content.
2. Differentiate between block-level and inline elements.
3. Utilize common HTML elements to create well-structured web pages.

### Introduction: The Foundation of Web Content

HTML elements are the fundamental building blocks that shape and structure all web pages. Just as a house relies on bricks and beams to stand, a webpage relies on HTML elements to define its content and layout. In this lesson, we’ll explore what HTML elements are, their types, and their role in building a well-structured webpage.

### Key Concepts

#### 1. **What are HTML Elements?**
- HTML elements are the basic components used to create the structure and content of a webpage. An element consists of:
  - **Opening Tag**: Denotes the start of an element, e.g., `<p>`.
  - **Content**: The text or other elements contained within the tags.
  - **Closing Tag**: Denotes the end of an element, e.g., `</p>`.

  **Example:**
  ```html
  <p>This is a paragraph element.</p>
  ```

  In this example, `<p>` is the opening tag, and `</p>` is the closing tag. The content is the text inside.

#### 2. **Block-level Elements**
- Block-level elements are used to create the main structure of a webpage. These elements take up the full width of the container, pushing other content to the next line.
  
  **Common Block-level Elements**:
  - `<div>`: A generic container element.
  - `<p>`: Defines a paragraph.
  - `<h1>` to `<h6>`: Headings, with `<h1>` being the most important.
  
  **Example:**
  ```html
  <div>
      <h1>Welcome to My Webpage</h1>
      <p>This is a block-level element.</p>
  </div>
  ```

  Here, the `<h1>` and `<p>` elements take up the full width and stack on top of each other.

#### 3. **Inline Elements**
- Inline elements do not start on a new line; they take up only as much space as their content requires. They are typically used for small portions of text or media inside block-level elements.
  
  **Common Inline Elements**:
  - `<span>`: A generic inline container for text.
  - `<a>`: Creates a hyperlink.
  - `<img>`: Embeds an image.

  **Example:**
  ```html
  <p>This is a <span>highlighted</span> word inside a paragraph.</p>
  ```

  In this example, the `<span>` element is inline and only takes up the space of the word it contains.

#### 4. **Void Elements (Self-Closing)**
- Void elements, also known as self-closing elements, do not have closing tags. These elements often insert content like images or line breaks.
  
  **Common Void Elements**:
  - `<img>`: Embeds an image.
  - `<br>`: Inserts a line break.
  - `<hr>`: Inserts a horizontal rule (line).
  
  **Example:**
  ```html
  <img src="image.jpg" alt="Sample Image">
  <hr>
  ```

  The `<img>` and `<hr>` elements are self-contained and do not need closing tags.

---

### Key Points
- HTML elements form the structure of a webpage, consisting of opening tags, content, and closing tags.
- Block-level elements (e.g., `<div>`, `<p>`, `<h1>`) create the main layout of a page, while inline elements (e.g., `<span>`, `<a>`) are used within text or blocks.
- Void elements, such as `<img>` and `<br>`, do not require closing tags.
- Using the right type of HTML elements helps ensure a well-structured and accessible webpage.