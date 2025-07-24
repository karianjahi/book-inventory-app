# 📚 Book Inventory App

The **Book Inventory App** is a simple, responsive web page that visually displays a list of books and their reading status using semantic HTML and advanced CSS techniques. The primary purpose of this project is to showcase the **power and flexibility of CSS attribute selectors** for styling structured content without relying on JavaScript or excessive class nesting.

## 🎯 Purpose

This project demonstrates how to use CSS **attribute selectors** to apply dynamic styling based on element attributes like `class`. The book table is visually enhanced by applying:

- Row background gradients based on book status
- Colored status badges using class-based attribute selectors
- Custom rating visualization using nested spans and class patterns

## 📁 File Structure

    ```
            book-inventory-app/
        ├── index.html # Main HTML structure for the book inventory table
        ├── styles.css # Styling with extensive use of attribute selectors
        ├── LICENSE # License for open-source sharing
        └── README.md # Project documentation (this file)
    ```


## 🧪 Features

- ✅ **CSS Attribute Selectors**
  - `[class="read"]`, `[class^="rate"]`, `[class~="two"]` and more
- 🎨 **Linear Gradients** applied via class-based targeting
- ⭐ **Visual Book Rating System**
  - Ratings shown with nested `<span>` elements styled conditionally
- 🧾 **Clear Semantic Markup** using `<table>`, `<thead>`, `<tbody>`, etc.
- 📐 **Responsive Layout** with modern styling

## 🖼️ Preview

A centered table showcasing books like:

| Title             | Author               | Category   | Status       | Rate     |
|------------------|----------------------|------------|--------------|----------|
| The Great Gatsby | F. Scott Fitzgerald  | Classic    | ✅ Read      | ⭐⭐⭐     |
| 1984             | George Orwell        | Dystopian  | 🔄 In Progress | ⭐⭐      |
| Clean Code       | Robert C. Martin     | Programming| 📖 To Read   | ☆☆☆      |

Each row is color-coded and visually distinct depending on reading status.

## 🧠 Key CSS Techniques Demonstrated

### Attribute Selectors Used

- Match exact class

tr[class="read"] { ... }

- Match class starting with "rate"

span[class^="rate"] { ... }

- Match class that includes the word "two"

span[class~="two"] > span:nth-child(1) { ... }


## Ratings Visualization
    
    span[class~="one"] > span:first-of-type { ... }
    span[class~="two"] > span:nth-child(1),
    span[class~="two"] > span:nth-child(2) { ... }
    span[class~="three"] > span { ... }
    
Each filled circle (styled <span>) represents a star in the book's rating.

## Status Badges
    
    tr[class="to-read"] span[class="status"] {
        border: 2px solid red;
        background-image: linear-gradient(to top, rgb(244, 52, 52), rgb(250, 103, 103));
    }
    

## 🔧 How to Use
1. Clone or download the repository

2. Open index.html in any modern browser

3. Inspect the code in styles.css to explore attribute selectors in action

    ```
    git clone https://github.com/karianjahi/book-inventory-app.git
    cd book-inventory-app
    open index.html  # or double-click the file
    ```
## ✅ License
This project is licensed under the MIT License.

## 🙏 Acknowledgments
Special thanks to **`freeCodeCamp`** for providing excellent web development tutorials and exercises that inspired this learning project.