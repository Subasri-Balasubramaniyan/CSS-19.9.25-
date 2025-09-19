🔹 1. CSS Pseudo-elements

Pseudo-elements let you style specific parts of an element.

Common Pseudo-elements:

::before → inserts content before an element.

::after → inserts content after an element.

::first-letter → styles the first letter.

::first-line → styles the first line.

::selection → styles selected text.

::marker → styles list item markers.

::placeholder → styles input placeholders.

👉 Example:

h1::before {
  content: "🔥 ";
}
p::first-letter {
  font-size: 2rem;
  color: red;
}
::selection {
  background: yellow;
  color: black;
}

🔹 2. CSS At-rules

At-rules start with @ and give instructions to the CSS engine.

Common At-rules:

@import → import external CSS

@media → responsive design

@supports → feature queries

@font-face → load custom fonts

@keyframes → define animations

@namespace → define XML namespace

@counter-style → custom list styles

@layer → cascade layers

👉 Example:

@media (max-width: 600px) {
  body { font-size: 14px; }
}

@supports (display: grid) {
  div { display: grid; }
}

🔹 3. CSS Cascade Layers (@layer)

Cascade layers let you control priority of CSS rules.

@layer reset, base, theme;

@layer reset {
  * { margin: 0; padding: 0; }
}
@layer base {
  h1 { color: blue; }
}
@layer theme {
  h1 { color: red; }
}


✅ Here, theme overrides base and reset.

🔹 4. CSS Functions

Functions in CSS perform calculations or transformations.

Common CSS Functions:

Colors

rgb(), rgba(), hsl(), hsla()

Math

calc(), min(), max(), clamp()

Transform

translate(), rotate(), scale(), skew()

Gradients

linear-gradient(), radial-gradient()

Shapes

circle(), ellipse(), polygon()

URL

url("image.png")

👉 Example:

.box {
  width: calc(100% - 50px);
  background: linear-gradient(to right, red, yellow);
  transform: rotate(15deg) scale(1.2);
}

🔹 5. CSS Fonts

Fonts define the typography of a webpage.

Font properties:

font-family → defines the font type

font-size → size of text

font-style → normal, italic, oblique

font-weight → normal, bold, 100–900

line-height → space between lines

letter-spacing → space between letters

text-transform → uppercase, lowercase, capitalize

👉 Example:

body {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 16px;
  line-height: 1.6;
}

🔹 6. Web Safe Fonts

Web safe fonts are pre-installed on most devices. They ensure consistent rendering.

Common Web Safe Fonts:
Sans-Serif

Arial

Helvetica

Verdana

Tahoma

Trebuchet MS

Serif

Times New Roman

Georgia

Garamond

Palatino Linotype

Monospace

Courier New

Lucida Console

Monaco

Consolas

👉 Example:

h1 {
  font-family: "Times New Roman", Times, serif;
}
p {
  font-family: Verdana, Geneva, sans-serif;
}


✅ Always provide fallback fonts (e.g., "Arial", sans-serif).

📝 Summary

Pseudo-elements → style parts of elements (::before, ::after, ::selection).

At-rules → special CSS instructions (@media, @supports, @keyframes).

Cascade layers → control stylesheet priority with @layer.

CSS functions → calculations, transforms, gradients, colors.

Fonts → define typography styles.

Web Safe Fonts → built-in fonts for consistency across devices.
