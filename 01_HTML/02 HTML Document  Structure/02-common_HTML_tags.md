## Common HTML Tags

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Identify and describe common HTML tags and their purposes.
2. Understand how to use these tags to structure a webpage.
3. Recognize the importance of semantic HTML in web development.

### Introduction: Building with HTML Tags

HTML tags are like the building blocks of a webpage. Just as bricks are used to create walls, HTML tags are used to create elements on a webpage. Each tag serves a specific purpose, helping browsers understand how to display content correctly.

### Common HTML Tags

Here’s a list of some of the most commonly used HTML tags, along with their purposes:

#### 1. **Headings (`<h1>` to `<h6>`)**
- Used to create headings and subheadings. `<h1>` is the largest and `<h6>` is the smallest.
  
  **Example:**
  ```html
  <h1>Main Title</h1>
  <h2>Subtitle</h2>
  ```

#### 2. **Paragraph (`<p>`)**
- Defines a block of text, creating a new paragraph.
  
  **Example:**
  ```html
  <p>This is a paragraph of text.</p>
  ```

#### 3. **Links (`<a>`)**
- Creates hyperlinks to other webpages or resources.
  
  **Example:**
  ```html
  <a href="https://www.example.com">Visit Example</a>
  ```

#### 4. **Images (`<img>`)**
- Embeds images in a webpage. It requires the `src` attribute to specify the image URL.
  
  **Example:**
  ```html
  <img src="image.jpg" alt="Description of image">
  ```

#### 5. **Lists**
   - **Unordered List (`<ul>`)**: Creates a bullet-point list.
   - **Ordered List (`<ol>`)**: Creates a numbered list.
   - **List Item (`<li>`)**: Defines an item in a list.
   
   **Example:**
   ```html
   <ul>
       <li>Item 1</li>
       <li>Item 2</li>
   </ul>
   ```

#### 6. **Divisions (`<div>`)**
- Groups content together and is often used for layout and styling.
  
  **Example:**
  ```html
  <div>
      <h2>Section Title</h2>
      <p>This is some content in a division.</p>
  </div>
  ```

#### 7. **Span (`<span>`)**
- A container for inline elements, useful for styling specific parts of text without breaking the flow.
  
  **Example:**
  ```html
  <p>This is a <span style="color: red;">red</span> word in a sentence.</p>
  ```

#### 8. **Table Tags**
- **Table (`<table>`)**: Creates a table.
- **Table Row (`<tr>`)**: Defines a row in a table.
- **Table Header (`<th>`)**: Defines a header cell in a table.
- **Table Data (`<td>`)**: Defines a standard cell in a table.
  
  **Example:**
  ```html
  <table>
      <tr>
          <th>Name</th>
          <th>Age</th>
      </tr>
      <tr>
          <td>John</td>
          <td>30</td>
      </tr>
  </table>
  ```

### Importance of Semantic HTML

Using the correct HTML tags helps improve accessibility and search engine optimization (SEO). Semantic tags convey meaning, making it easier for search engines and assistive technologies to understand your content.

---

### Key Points
- HTML tags are essential for structuring a webpage and defining its content.
- Common tags include headings, paragraphs, links, images, lists, divisions, spans, and tables.
- Using semantic HTML is crucial for accessibility and improving user experience on the web.