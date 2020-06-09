# HTML Links, CSS Layout, JS Functions

- Writing Links
`<a href="www.google.com">Google</a>`

| Relative Link Type | Example |
| ------------- | ------------- |
|Same Folder | <a href="reviews.html">Reviews</a> |
|Child Folder | <a href="music/listings.html">Listings</a> |
|Grandchild Folder | <a href="movies/dvd/reviews.html">Reviews</a> |
|Parent Folder | <a href="../index.html">Home</a> |
|GrandParent Folder |  <a href="../../index.html">Home</a> |

### Email Links

`<a href="mailto:jon@example.org">Email Jon</a>`
- You can create links to open email programs with an email address in the "to" field.

### Opening Links in a New Window

`<a href="http://www.imdb.com" target="_blank">Internet Movie Database</a> (opens in new window)`

### Linking to a Specific Part of the Same Page

`<h2 id="prologue">Prologue</h2>`
`<a href="#prologue">Prologue</a><br /><br />`

### Linking to a Specific Part of Another Page

`<a href="http:/www.htmlandcssbookcom/#bottom">`

## Key Concepts in Positioning Elements
## Building Blocks
- Block-level elements : start on a new line
  - Examples include:
`<h1> <p> <ul> <li>`
- Inline elements : flow in between surrounding text
  - Examples include:
`<img> <b> <i>`

## Containing Elements
If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

## Controlling the Position of Elements
![](https://chenhuijing.com/assets/images/posts/css-positioning.jpg)

**Notes:**
1. `<div>` elements are often used as containing elements to group together sections of a page.
2. Pages can be fixed width or liquid (stretchy) layouts.
3. You can include multiple CSS files in one page.

## FUNCTIONS, METHODS & OBJECTS 

**Functions** : series of statements together to perform a specific task. 

### Declaring functions :
`function sayHello(){`
  `console.log('Hello');`
`}`
### Calling a function :
`sayHello();`

### FUNCTION EXPRESSION :
`var ar ea = f unction(width, height) {`
`return width * height;`
`} ; `
