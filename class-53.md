# Routing

![](https://blog.theodo.com/static/0ffcd364876dbe20a4a67ec9332d686e/50383/react-router-workflow.png)

- React Router v4 is a pure React rewrite of the popular React package. Previous versions of React Router used configuration disguised as pseudo-components and could be difficult to understand. With v4, everything is “just components”.

- For browser based projects, there are <BrowserRouter> and <HashRouter> components. The <BrowserRouter> should be used when you have a server that will handle dynamic requests (knows how to respond to any possible URI), while the <HashRouter> should be used for static websites (where the server can only respond to requests for files that it knows about).

### Discussion

- When a component “wraps” another component, how does the child component’s output get rendered?
    - You can access this (the instance of the WrappedComponent) with a ref, but you will need a full initial normal render process of the WrappedComponent for the ref to be calculated, that means that you need to return the WrappedComponent element from the HOC render method, let React do it’s reconciliation process and just then you will have a ref to the WrappedComponent instance.
- When a component “wraps” another component, how does the child component’s output get rendered?
    - No, the parent have access to the props/state of the child.

### Terms

- props.children : it includes the component children in the rendered result.

- composition : composition is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these components are, they can be used in building many other components.

### Resources

- [router api](https://reactrouter.com/web/api)
- [tutorial](https://blog.pshrmn.com/simple-react-router-v4-tutorial/)