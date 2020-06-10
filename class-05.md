# HTML Images; CSS Color & Text

## Images

`<img src="images/quokka.jpg" alt="A family of quokka" title="The quokka is an Australian marsupial that is similar in size to the domestic cat." />`

- `<img>` : To add an image to the page.
- `src` : a relative URL pointing to an image 
- `alt` : a text description of the image which describes the image.
- `title` : to provide additional information about the image.
- `height` : This specifies the height of the image in pixels.
- `width`: This specifies the width of the image in pixels.

## Where to Place Images in Your Code?

1. before a paragraph The paragraph starts on a new line after the image.
2. inside the start of a paragraph The first row of text aligns with the bottom of the image.
3. in the middle of a paragraph The image is placed between the words of the paragraph that it appears in.

- `<figure>` element to contain images and their caption.
- `<figcaption>` element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.

## Color

#### You can specify any color in CSS in one of three ways:

`/* color name */`
`h1 {color: DarkCyan;}`
`/* hex code */`
`h2 {color: #ee3e80;}`
`/* rgb value */`
`p {color: rgb(100,100,90);}`

**Note:** Every color on a computer screen is created by mixing amounts of red,
green, and blue. 

#### opacity, rgba
- `p.one {`
    `background-color: rgb(0,0,0);`
    `opacity: 0.5;}`
- alpha: This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.

#### HSL Colors 
- (Hue, saturation, Lightness).

## Text
![](https://htmldog.com/figures/weightStyle.gif)

**Note** : When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer

| Technique | what it does |
| ------------- | ------------- |
| font-family | allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies. |
| font-size| enables you to specify a size for the font. |
| Font-Face | Commercial services give users access to a wider range of fonts using @font-face.|

- Unites of Type size : Pixels, Percentages, Ems.

- font-weight : 
1. `normal` : This causes text to appear at a normal weight.
2. `bold` : This causes text to appear bold.

- font-style :
1. `normal` : This causes text to appear in a normal style.
2. `italic`: This causes text to appear italic.
3. `oblique`: This causes text to appear oblique.

- text-transform :
1. `uppercase` : This causes the text to appear uppercase.
2. `lowercase` : This causes the text to appear lowercase.
3. `capitalize`: This causes the first letter of each word to appear capitalized.

- text-decoration :
1. `none` : This removes any decoration already applied to the text.
2. `underline`: This adds a line underneath the text.
3. `overline` : This adds a line over the top of the text.
4. `line-through`: This adds a line through words.
5. `blink`: This animates the text to make it flash on and off.

- text-align :
1. `left` : This indicates that the text should be left-aligned.
2. `right` : This indicates that the text should be right-aligned.
3. `center` : This allows you to center text.
4. `justify` : This indicates that every line in a paragraph, except the last line, should be set to take up the full width of the containing box.

- vertical-align :
`baseline, sub, super, top, text-top, middle, bottom, text-bottom`

- `:link` : This allows you to set styles for links that have not yet been visited.
- `:visited`: This allows you to set styles for links that have been clicked on.
- `:hover` :  when a user hovers over an element with a pointing device such as a mouse. 
- `:active` : This is applied when an element is being activated by a user.
- `:focus` :  This is applied when an element has focus.  