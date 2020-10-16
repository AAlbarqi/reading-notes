# Context API

- Context provides a way to pass data through the component tree without having to pass props down manually at every level.

- Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

- Context is designed to share data that can be considered “global” for a tree of React components.

- Context is primarily used when some data needs to be accessible by many components at different nesting levels. 

- This inversion of control can make your code cleaner in many cases by reducing the amount of props you need to pass through your application and giving more control to the root components.

![](https://joecortopassi.com/images/react_context_diagram.png)

- React.createContext : Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.
`const MyContext = React.createContext(defaultValue);`

- The defaultValue argument is only used when a component does not have a matching Provider above it in the tree.

- Context.Provider : Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes.
`<MyContext.Provider value={/* some value */}>`

- The contextType property on a class can be assigned a Context object created by React.createContext(). This lets you consume the nearest current value of that Context type using this.context. 

- Context.Consumer : A React component that subscribes to context changes. This lets you subscribe to a context within a function component.

- Context.displayName : Context object accepts a displayName string property. React DevTools uses this string to determine what to display for the context.

### Term

- reducer : a pure function that takes the previous state and an action, and returns the next state. It's called a reducer because it's the type of function you would pass to Array.

### Resources 

[Example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)