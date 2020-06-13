# JS Object Literals; The DOM

### WHAT IS AN OBJECT?
- Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. 
- IN AN OBJECT: 
1. VARIABLES BECOME KNOWN AS PROPERTIES.
2. FUNCTIONS BECOME KNOWN AS METHODS 
![](https://lh3.googleusercontent.com/proxy/suni_g6uS4oT-juZZG_oImUCu0umNp3MSxrtsBMwlt7WuM_dfDfA3pInWJyH3ALQg_sTf9pUqvuOU_-UdW_mn3vA)
![](https://cdn.hashnode.com/res/hashnode/image/upload/v1576395857500/Him6j7txy.png)

### How to access an object?
1. dot notation:
   - `var hotelName = hotel.name;`
2. square brackets:
   - `var hotelName = hotel['name'];`

### The Document Object Model (DOM) 
It how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

- As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.
1. THE DOCUMENT NODE
2. ELEMENT NODES
3. ATTRIBUTE NODES
4. TEXT NODES

- Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes. 

### Caching DOM queries 
 DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes. 
#### METHODS THAT RETURN A SINGLE ELEMENT NODE: 
1. getElementByld('id');
   - `get ElementByld('one') `
2. querySel ector('css selector')
   - `querySelector('l i . hot ' )`
#### METHODS THAT RETURN ONE OR MORE ELEMENTS (AS A NODELIST):
1. getElementsByClassName('class')
   - `getElementsByCl assName ('hot');`
2. getElementsByTagName('tagName') 
   - `getElementsByTagName('li');`
3. querySelectorAll('css select or')
   - `querySelectorAll('li.hot');`

#### THE item() METHOD
Nodelists have a method called item() which will return an individual node from the
Node list. 
- `var elements = document.getElementsByClassName('hot')`
- `if (elements.length>= 1) {`
- `var firstltem = elements.item(O);}` 

#### Traversing the DOM
When you have an element node, you can select another element in relation to it using these properties.
`parentNode` , `previousSibling` , `nextSibling` , `firstChild` , `lastChild`
- The **textContent** property allows you to collect or update just the text that is in the containing element (and its children). 
We can add content, Using :
1. textContent
2. innerText  
3. document.write()

`document.write()`: a simple way to add content that was not in the original source code to the page, but its use is rarely advised. 

- Using the **innerHTML** property, you can accessand amend the contents of an element,
including any child elements.
   - GET CONTENT: 
   `var elContent = document.getElementByld('one').innerHTML;`
   - SET CONTENT:
   `document .getElementByld('one').innerHTML = elContent;`
**Note :** If you add HTML to a page using i nnerHTML (or several jQuery methods), you need to be aware of Cross-Site Scripting Attacks or XSS; otherwise, an attacker could gain access to your users' accounts. 

- Attribute Node : 
1. getAttribute();
2. hasAttribute();
3. setAttribute();
4. removeAttribute();
