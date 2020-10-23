# Redux - Additional Topics

- The Redux Toolkit package is intended to be the standard way to write Redux logic.

- we can replace the plain Redux `createStore` function with RTK's `configureStore`. This will automatically set up the Redux DevTools Extension for the app.

Redux Toolkit: we can use Redux and RTK from a plain JS script tag in an HTML page, without using React, NPM, Webpack, or any build tools.

- createSlice takes an options object as its argument, with these options:
    - name: prefix for generated action types
    - initialState: the initial state value for the reducer
    - reducers: an object, where the keys will become action type strings, and the functions are reducers that will be run when that action type is dispatched. 

- Alternative State Managers:
    - Hookstate: The simple but incredibly fast and flexible state management that is based on React state hook
    - MobX: a simple, scalable and battle tested state management solution.

### Terms

- middleware: Middleware provides a way to interact with actions that have been dispatched to the store before they reach the store's reducer.

- thunk: a middleware that lets you call action creators that return a function instead of an action object.