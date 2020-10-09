# Component Based UI

- JSX, is a syntax extension to JavaScript. it is used with React to describe what the UI should look like. 
- JSX produces React “elements”. to be rendered to the DOM.
- React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

![](https://hackernoon.com/hn-images/1*jhD-rWxuFvo17Q1Mw6LuEw.jpeg)

- Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

- Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

To render a React element into a root DOM node, pass both to ReactDOM.render():
`ReactDOM.render(element, document.getElementById('root'));`

- React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.

With our knowledge so far, the only way to update the UI is to create a new element, and pass it to ReactDOM.render().

`const element = <h1>Hello, world!</h1>;`


### Discussion 

- Name 5 Javascript UI Frameworks (other than React)
    - Vue
    - Angular
    - Ember
    - Backbone.js
    - Next.js
- What’s the difference between a framework and a library?
    - A library is just a collection of class definitions. A framework is normally more complex. It defines a skeleton where the application defines its own features to fill out the skeleton.

### Term

- Rendering : Render refers to show output in browser and @JavaScript (programming language) utilize the document object to manipulate DOM elements.

- Templates : a chunk of HTML that you need to inject onto the page.

- State : State describes the status of the entire program or an individual object. It could be text, a number, a boolean, or another data type.

### Resources

- [react](https://reactjs.org/docs/hello-world.html)
- [sass](https://devhints.io/sass)
- [react cheatsheet](https://devhints.io/react)
- [another CS](https://reactcheatsheet.com/)