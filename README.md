# CSS Selectors & Specificity Demonstration

This project demonstrates various CSS selector techniques, including element selectors, class selectors, ID selectors, pseudo-classes (`:first-child`, `:nth-child`), combinators (child selectors `>`), and inline styling.

---

## 📁 Project Structure

```
.
├── index.html   # Main HTML document containing structured semantic markup
└── style.css    # External stylesheet containing custom CSS rules
```

---

## 📄 Overview of Files

### 1. `index.html`
- **Header Section (`<header id="headings">`)**:
  - Contains `<h1>`, `<h2>`, and `<h4>` headings.
  - Demonstrates usage of classes (`class="head"`), IDs (`id="bglime"`), and inline styling (`<span style="color: red">`).
- **Main Content (`<main>`)**:
  - Uses `<article>` tags containing `<p>` elements to illustrate paragraph styling.
  - Contains a `<section>` with an unordered list (`<ul>`) and ordered list (`<ol>`) to showcase link and list-item targeting using CSS pseudo-classes.

### 2. `style.css`
- **Global / Body**:
  - `body`: Sets background color to orange/coral (`#f9844a`).
- **Class & ID Selectors**:
  - `.head`: Targets headings with dark blue text (`color: darkblue`).
  - `#bglime`: Sets background color to light green (`background-color: lightgreen`).
  - `#para`: Styles targeted paragraph with green text and `20px` font size.
  - `#para span`: Targets nested `<span>` with black text and enlarged `30px` font size.
- **Structural Combinators & Pseudo-Classes**:
  - `section > ul > li`: Sets unordered list text color to white.
  - `section > ol > li`: Sets ordered list text color to black.
  - `section ul li:first-child a`: Applies yellow background to the first hyperlink.
  - `section li:nth-child(2) a`: Applies semi-transparent blue background to the second hyperlink.
  - `section ol li:nth-child(2)`: Colors the 2nd ordered list item blue.
  - `section ol li:nth-child(3)`: Colors the 3rd ordered list item red.

---

## 🎯 Key Concepts Covered

| Concept | Description | Example |
| :--- | :--- | :--- |
| **Element Selector** | Targets elements by tag name | `p { color: white; }` |
| **Class Selector** | Targets elements using `class` attribute | `.head { color: darkblue; }` |
| **ID Selector** | Targets unique elements using `id` attribute | `#bglime { background-color: lightgreen; }` |
| **Child Combinator** | Targets immediate child elements | `section > ul > li` |
| **Nth-Child Selector** | Targets elements based on index position | `ol li:nth-child(2)` |
| **First-Child Selector** | Targets the first element among siblings | `ul li:first-child a` |

---

## 🚀 How to Run

1. Clone or download the project files.
2. Ensure `index.html` and `style.css` are in the same folder.
3. Open `index.html` in any web browser to view the rendered page.
