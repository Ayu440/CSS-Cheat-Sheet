# CSS-Cheat-Sheet
# CSS Cheatsheet

## What is CSS?
CSS (Cascading Style Sheets) is a stylesheet language used to control the presentation and layout of HTML documents.

---

## CSS Syntax
```css
selector {
  property: value;
}
```
### Example:
```css
p {
  color: blue;
  font-size: 16px;
}
```

---

## CSS Selectors

### Universal Selector
```css
* {
  margin: 0;
  padding: 0;
}
```

### Type Selector
```css
h1 {
  color: red;
}
```

### Class Selector
```css
.className {
  font-size: 14px;
}
```

### ID Selector
```css
#idName {
  background-color: yellow;
}
```

### Attribute Selector
```css
input[type="text"] {
  border: 1px solid black;
}
```

### Group Selector
```css
h1, h2, p {
  color: green;
}
```

### Pseudo-classes
```css
a:hover {
  color: orange;
}
```

### Pseudo-elements
```css
p::first-line {
  font-weight: bold;
}
```

---

## Colors

### Named Colors
```css
color: red;
```

### Hexadecimal
```css
color: #ff5733;
```

### RGB
```css
color: rgb(255, 87, 51);
```

### RGBA
```css
color: rgba(255, 87, 51, 0.5);
```

---

## Text Styling
```css
h1 {
  font-family: Arial, sans-serif;
  font-size: 24px;
  color: black;
  text-align: center;
  text-transform: uppercase; /* uppercase, lowercase, capitalize */
  text-decoration: underline; /* none, underline, overline, line-through */
  line-height: 1.5; /* Adjusts spacing between lines */
  letter-spacing: 2px; /* Adjusts spacing between letters */
  word-spacing: 4px; /* Adjusts spacing between words */
}
```

---

## Box Model
```css
div {
  width: 100px;
  height: 100px;
  padding: 10px;
  border: 2px solid black;
  margin: 20px;
}
```

### Components:
1. **Content**: The actual content inside the box.
2. **Padding**: Space between the content and the border.
3. **Border**: Surrounds the padding (or content if there’s no padding).
4. **Margin**: Space outside the border.

---

## Positioning

### Static (Default)
```css
position: static;
```

### Relative
```css
position: relative;
top: 10px;
left: 10px;
```

### Absolute
```css
position: absolute;
top: 20px;
right: 20px;
```

### Fixed
```css
position: fixed;
bottom: 0;
right: 0;
```

### Sticky
```css
position: sticky;
top: 50px;
```

---

## Flexbox
```css
.container {
  display: flex;
  justify-content: center; /* flex-start, flex-end, space-between, space-around, space-evenly */
  align-items: center; /* flex-start, flex-end, stretch */
  flex-direction: row; /* row-reverse, column, column-reverse */
  gap: 10px; /* Space between items */
}
```

---

## Grid
```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr); /* Three equal columns */
  grid-template-rows: auto; /* Rows adjust based on content */
  gap: 10px;
}
```

---

## Backgrounds
```css
body {
  background-color: #f0f0f0;
  background-image: url('image.jpg');
  background-size: cover; /* cover, contain, auto */
  background-position: center; /* top, bottom, left, right */
  background-repeat: no-repeat; /* repeat, repeat-x, repeat-y */
}
```

---

## Borders
```css
div {
  border: 2px solid black; /* solid, dashed, dotted, double */
  border-radius: 10px; /* Rounded corners */
}
```

---

## Transitions
```css
button {
  transition: background-color 0.3s ease-in-out;
}
button:hover {
  background-color: blue;
}
```

---

## Animations
```css
@keyframes example {
  0% { transform: translateX(0); }
  50% { transform: translateX(50px); }
  100% { transform: translateX(0); }
}
div {
  animation: example 2s infinite;
}
```

---

## Media Queries
```css
@media (max-width: 768px) {
  body {
    background-color: lightblue;
  }
}
```

---

## Z-Index
```css
div {
  position: absolute;
  z-index: 10; /* Higher number = higher layer */
}
```

---

## Overflow
```css
div {
  overflow: hidden; /* visible, hidden, scroll, auto */
}
```

---

## CSS Variables
```css
:root {
  --main-color: #3498db;
}
h1 {
  color: var(--main-color);
}
```

---

## Shadows

### Box Shadow
```css
div {
  box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
}
```

### Text Shadow
```css
h1 {
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
}
