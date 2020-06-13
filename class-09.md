# Forms and Events

- The best known form on the web is probably the search box that sits right in the middle of Google's homepage.

- Form Controls :
1. ADDING TEXT:
- Text input (single-line) : `<input type="text" name="username" size="15" maxlength="30" />`
- Password input : `<input type="password" name="password" size="15" maxlength="30" />`
- Text area (multi-line) : `<textarea name="comments" cols="20" rows="4">Enter your comments...</textarea>`
- Date Input : `<input type="date" name="depart" />`
- Email & URL Input: `<input type="email" name="email" />`
- Search input: `<input type="search" name="search" />`
2. Making Choices:
- Radio buttons : `<input type="radio" name="genre" value="rock" checked="checked" /> Rock`
- Checkboxes : `<input type="checkbox" name="service" value="itunes" checked="checked" /> iTunes`
- Drop-down boxes : `<select name="devices">`
 `<option value="ipod">iPod</option>`
 `<option value="radio">Radio</option>`
 `</select>`
3. Submitting Forms:
- Submit buttons : `<input type="submit" name="subscribe" value="Subscribe" />`
- Image buttons : `<input type="image" src="images/subscribe.jpg" width="100" height="20" />`
4. Uploading Files:
- File upload : `<input type="file" name="user-song" />`

## Form Structure
- `<form>` : Form controls live inside a <form> element.
- `action` : Its value is the URL for the page on the server that will receive the information in the form when it is submitted.
- `method` : Forms can be sent using one of two methods: get or post.

### Labelling Form Controls
- each form control should have its own <label> element as this makes the form accessible to vision-impaired users.
`<label>Age: <input type="text" name="age" /></label>`

### Grouping Form Elements
- `<fieldset>`: You can group related form controls together inside the <fieldset> element. This is particularly helpful for longer forms.
- `<legend>` : The <legend> element can come directly after the opening <fieldset> tag and contains a caption which helps identify the purpose of that group of form controls.

## Lists, Tables and Forms
- Bullet Point Styles : `list-style-type`
- Unordered Lists:
For an unordered list you can use the following values: none, disc, circle, square.
- Ordered Lists
For an ordered (numbered) list you can use the following values: decimal(1 2 3), decimal-leading-zero(01 02 03), lower-alpha(a b c), upper-alpha(A B C), lower-roman
(i. ii. iii.), upper-roman(I II III).

- Images for Bullets : `list-style-image`
- `ul {list-style-image: url("images/star.png");}`

- Positioning the Marker : `list-style-position`
- `ul.illuminations {list-style-position: outside;}`
- `ul.season {list-style-position: inside;}`

- Table Properties :
| property  |  what it does |
| ------------- | ------------- |
| width | to set the width of the table padding to set the space between the border of each table cell and its content |
| text-transform |to convert the content of the table headers to uppercase
| letter-spacing, font-size | to add additional styling to the content of the table headers |
| border-top, border-bottom | to set borders above and below the table headers
| text-align | to align the writing to the left of some table cells and to the right of the others |
| background-color | to change the background color of the alternating table rows |
| :hover | to highlight a table row when a user's mouse goes over it|

- Border on Empty Cells : empty-cells
`table.one {empty-cells: show;}`

- Cursor Styles : cursor 
- Here are the most commonly used values for this property: auto, crosshair, default, pointer, move, text, wait, help, url("cursor.gif");

## Events 
When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling. 
1. Select t he element node(s) you want the script to respond to. 
2. Indicate which event on the selected node(s) will trigger the response. 
3. State the code you want to run when the event occurs. 


#### Diffrenet Handlers : 
- HTML EVENT HANDLER ATTRIBUTES (DO NOT USE)  : `<input type="text" i d="username" onbl ur="checkUsername()" /> `
- TRADITIONAL DOM EVENT HANDLERS : `element.onevent = functionName ;`

#### EVENT LISTENERS:
- `element.addEventlistener('event', functionName [,Boolean]) ;` 
#### USING EVENT LISTENERS:
- `elUsername.addEventlistener('blur' , checkUsername , false) ;`

##### CHANGING DEFAULT BEHAVIOR
- For that we use `preventDefault()` or `stopPropagation()`;

| Event  |  what it does |
| ------------- | ------------- |
|LOAD | used to trigger scripts that access the contents of the page. |
|FOCUS & BLUR| the focus/blur event fires for that DOM node. |
|Click |  fire for the element that the mouse is currently over. |
|submit | fires on the node representing the <form> element.|