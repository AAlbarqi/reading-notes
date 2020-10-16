# Hooks API

- Hooks are functions that let you “hook into” React state and lifecycle features from function components. 

- Hooks are a new addition in React that lets you use state and other React features without writing a class. 

- Hooks let you use React features (like state) from a function — by doing a single function call. React provides a few built-in Hooks exposing the “building blocks” of React: state, lifecycle, and context.

- Hooks let us organize the logic inside a component into reusable isolated units.
- Hooks apply the React philosophy (explicit data flow and composition) inside a component, rather than just between the components. 
- Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props.
- Adopting Hooks could reduce your bundle size because code using Hooks tends to minify better than equivalent code using classes. 

- Hooks are fully encapsulated — each time you call a Hook, it gets isolated local state within the currently executing component.

![](https://miro.medium.com/max/684/1*R-oovJm4IQBLDjZy6DvbBg.png)

- You can write custom Hooks that cover a wide range of use cases like form handling, animation, declarative subscriptions, timers.

- `useState` is a Hook. We call it inside a function component to add some local state to it. React will preserve this state between re-renders. useState returns a pair: the current state value and a function that lets you update it.
-   `const [age, setAge] = useState(42);`

- The Effect Hook, `useEffect`, adds the ability to perform side effects from a function component. It serves the same purpose as componentDidMount, componentDidUpdate, and componentWillUnmount in React classes, but unified into a single API. 
-   `useEffect(() => { document.title = `You clicked ${count} times`; });`

- Five Important Rules for Hooks:
    1. Never call Hooks from inside a loop, condition or nested function
    2. Hooks should sit at the top-level of your component
    3. Only call Hooks from React functional components
    4. Never call a Hook from a regular function
    5. Hooks can call other Hooks

### Term

- Composition : is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. 

- Children / Child Components : Children allow you to pass components as data to other components, just like any other prop you use.

- Hash Routing : allows you to build one-page apps where the navigation is done by changing the hash, so the browser does not have to reload the page. 

- Link Routing : React-Router provides the <Link> and <NavLink> components, which allow you to navigate to different routes.

### Resources:

[Hooks](https://reactjs.org/docs/hooks-overview.html)
[Hooks API](https://reactjs.org/docs/hooks-reference.html)