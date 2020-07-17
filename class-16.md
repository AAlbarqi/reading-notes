#  jQuery, Events, and The DOM

jQuery offers a simple way to achieve a variety of common
JavaScript tasks quickly and consistently, across all major
browsers and without any fallback code needed. $() is a shortcut for the jQuery () function. 

- Function(Creates jQuery Objects) `$('li.hot')`
- `$(' :header').addClass('headline');` : To add class.
- `$('li:lt(3) ').hide().fadeln(lSOO);` : To hide element.
- `$('li').on('click', function() {$(this).remove();}); ` : To invoke a function when li is clicked.

##### A matched set/JQUERY selection 
- single element : $('ul')
- multiple elements : $('li')

When you create a selection with jQuery, it stores a reference to the corresponding nodes in the DOM tree. It does not create copies of them.

###### Chaining 
example : `$('li[id!="one"]').hide().delay(500).fadeln(1400);`

##### Checking a page is ready to work with
- `$(document).ready(function(){//code});`
- a shortcut : `$(function(){//code});`

##### Getting element content
- The .html() and .text() methods both retrieve and update the content of elements. 
- `html()` This method gives every element in the matched set the same new content. The new content may include HTML.
- `text()` This method gives every element in the matched set the same new text content. Any markup would be shown as text. 
- `remove()` This method removes all of the elements in the matched set. 
- `replaceWith()` This method replaces every
element in a matched set with new content. It also returns the replaced elements. 

##### Changing elements
- `before()` This method inserts content before the selected element(s) .
- `prepend()` This method inserts content inside the selected element(s), after the opening tag.
- `after()` This method inserts content after the selected element(s).
- `append()` This method inserts content inside the selected element(s), before the closing tag. 

##### Getting and Setting attribute values
- `attr()` This method can get or set a
specified attribute and its value.
- `removeAttr()` This method removes a specified
attribute (and its value). 
- `addClass()` This method adds a new value to the existing value of the class attribute.
- `removeClass()` This method removes a value from the class attribute, leaving any other class names within that attribute intact. 

##### GETTING & SETTING CSS PROPERTIES
The . css () method lets you retrieve and set the values of CSS properties. 
`$('li') .css( 'background- color' , '1272727' ); `

##### WORKING WITH EACH ELEMENT IN A SELECTION

jQuery allows you to recreate the functionality
of a loop on a selection of elements, using the
.each () method. 

- `each()` Allows you to perform one or more statements on each of the items in the selection of elements that is returned by a selector - rather like a loop in JavaScript. 
- `this` or `$(this)` As the .each() method goes through the elements in a selection, you can access the current element using the this keyword. 

##### EVENT METHODS
The .on() method is used to handle all events. 
`$('li').on('click', function(){$(this).addClass( 'complete'); }) ; `
- . on(events[, selector][, data], function(e) ); 

##### Ways to include jQuery in your page
- LOADING JQUERY FROM A CDN 
`<script src="//ajax.googleapis.com/ajax/l ibs/jquery/1.10.2/jquery.min.js"></script> `

## 6 Reasons for Pair Programming
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness

