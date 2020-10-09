# Component Composition

![](https://i.pinimg.com/originals/6a/28/34/6a28340a376c71d91b1193b2d1a80bdb.jpg)

- The component lifecycle: it details the life of a component. A component can only be in one stage at a time. It starts with mounting and moves onto updating. It stays updating perpetually until it gets removed from the virtual DOM. Then it goes into the unmounting phase and gets removed from the DOM.

- Mounting: Since class-based components are classes, the first method that runs is the constructor method. Typically, the constructor is where you would initialize component state.
Next, the component runs the getDerivedStateFromProps. Now we come to the render method which returns your JSX. Now React “mounts” onto the DOM. Lastly, the componentDidMount method runs. Here is where you would do any asynchronous calls to databases or directly manipulate the DOM if you need.

- Updating : This phase is triggered every time state or props change. Like in mounting, getDerivedStateFromProps is called (but no constructor this time!). Next shouldComponentUpdate runs. Here you can compare old props/state with the new set of props/state. You can determine if your component should re-render or not by returning true or false. This can make your web app more efficient by cutting down on extra re-renders. If shouldComponentUpdate returns false, this update cycle ends.If not, React re-renders and getSnapshotBeforeUpdate runs afterwards. This method has limited use as well. React then runs componentDidUpdate. Like componentDidMount you can use it to make any async calls or manipulate the DOM.

- The React docs say that you can use props.children on components that represent ‘generic boxes’ and that ‘don’t know their children ahead of time’.

- Composition vs Inheritance : 
    - Containment : components don't know their children ahead of time.
    - Specialization : components as being 'special cases' of other components.

### Discussion

- Can a parent component access the state of a child component?
    - you can declare a ref in the parent component, then pass it as a ref attribute to the child
- What can be passed along in a prop variable?
    - you can pass dynamic data to your component.

### Terms
- component props : stands for properties and is being used for passing data from one component to another.

- component state : The state object is where you store property values that belongs to the component. When the state object changes, the component re-renders.

- application state : the state at which an application resides with regards to where in a program is being executed and the memory that is stored for the application.

### Resources

- [concepts](https://www.freecodecamp.org/news/these-are-the-concepts-you-should-know-in-react-js-after-you-learn-the-basics-ee1d2f4b8030/)
- [props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)
- [testing library](https://testing-library.com/docs/react-testing-library/example-intro)
- [react-if](https://www.npmjs.com/package/react-if)
- [Async utilities](https://testing-library.com/docs/dom-testing-library/api-async)
