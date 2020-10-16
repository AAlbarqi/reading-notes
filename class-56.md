# Custom Hooks

- A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks.
- We can decide what it takes as arguments, and what it should return.
- Custom Hooks are a mechanism to reuse stateful logic, but every time you use a custom Hook, all state and effects inside of it are fully isolated.
- We make custom hooks, to make our code cleaner and single liner on final usage. It must be not redundant or to keep it DRY.

- Async React Hooks: 
 Hooks with Async-Await, We cannot use 'async' keyword with 'useEffect' callback method. It will result in race conditions.

- useHooks:
    - useFirestoreQuery : makes it easy to subscribe to data in your Firestore database without having to worry about state management.
    - useMemoCompare : This hook is similar to useMemo, but instead of passing an array of dependencies we pass a custom compare function that receives the previous and new value.
    - useAsync :  to indicate to users the status of any async request. 
    - useRequireAuth : a way to redirect the user if they are signed out and trying to view a page that should require them to be authenticated.
    - useRouter : exposes just the data and methods we need. In this recipe we show how easy it is to compose multiple hooks and combine their returned state into a single object. 
    - useAuth : have a bunch of components that need to render different depending on whether the current user is logged in and sometimes call authentication methods like signin, signout.
    - useEventListener : handles checking if addEventListener is supported, adding the event listener, and removal on cleanup.

- `useReducer` : An alternative to useState. Accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method.

- `useReducer` is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. 

### Terms

- state hook
- effect hook
- reducer hook

### Resources

- [Hooks guide](https://www.telerik.com/kendo-react-ui/react-hooks-guide/#toc-custom-react-hooks)
- [use Hooks](https://usehooks.com/)
- [Hooks list](https://github.com/rehooks/awesome-react-hooks)