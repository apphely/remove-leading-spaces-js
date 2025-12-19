# Remove Leading Spaces from Paragraphs (JavaScript)

A lightweight and easy-to-use JavaScript snippet that removes unnecessary leading spaces from `<p>` elements inside a specified container.  
Perfect for cleaning up imported, scraped, or auto-generated HTML content without modifying the original source code.

---

## 🚀 Features

- Removes unwanted leading whitespace from paragraphs
- Improves text readability and layout consistency
- Works instantly in the browser
- Fully customizable (ID, class, or element-based targeting)
- Compatible with all modern browsers
- No dependencies required

---

## 📌 Use Cases

This script is especially useful for:

- Novel reader websites
- Blogs with imported or copied content
- Auto-generated HTML pages
- Scraped or translated text with formatting issues
- Improving copy-paste behavior and visual alignment

---

## 🧩 The Code

```js
// Select an element with a specific id
var attribute = document.getElementById("novel_honbun");

// use this for class:
// var attribute = document.getElementsByClassName("novel_text");

if (attribute) {
    // Select all <p> elements
    var paragraphs = attribute.getElementsByTagName("p");
    
    for (var i = 0; i < paragraphs.length; i++) {
        paragraphs[i].innerText = paragraphs[i].innerText.trimLeft();
    }
}
