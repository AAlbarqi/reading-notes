# More CSS Layout

### Key Concepts in Positioning Elements
- Block-level elements: start on a new line
    - Examples include: `<h1> <p> <ul> <li>`
- Inline elements: flow in between surrounding text
    - Examples include: `<img> <b> <i>`

* **Containing Elements**: If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

* Controlling the Position of Elements : positioning schemes are :
1. Normal flow : `position:static`
2. Relative Positioning : `position:relative`
3. Absolute positioning : `position:absolute`
4. Fixed Positioning : `position:fixed`
5. Floating Elements : `float`

- The `z-index` property allows you to control which box appears on top (overlapping elements).
- Clearing Floats : `clear` property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box.

#### CREATING Multi-Column Layouts with Floats :
1. `width` This sets the width of the columns.
2. `float` This positions the columns next to each other.
3. `margin` This creates a gap between the columns.
