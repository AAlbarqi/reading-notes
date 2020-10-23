# Redux - Asynchronous Actions

When you call an asynchronous API, that usually requires a change in the application state; to do that, you need to dispatch normal actions that will be processed by reducers synchronously. 

- For any API request you'll want to dispatch at least three different kinds of actions:

    - An action informing the reducers that the request began.
    - An action informing the reducers that the request finished successfully.
    - An action informing the reducers that the request failed.

- It is not immediately clear what information describes the state of an asynchronous application, and how to organize it in a single tree. You'll need to figure out what sorts of lists your app can show. You want to store them separately in the state, because this way you can cache them and only fetch again if necessary.

- For every list of items, you'll want to store `isFetching` to show a spinner, `didInvalidate` so you can later toggle it when the data is stale, `lastUpdated` so you know when it was fetched the last time, and the items themselves. 

- Redux Thunk : a middleware library that allow for side effects and asynchronous actions.

![](https://miro.medium.com/max/800/1*uHumlKU6fado6sOF2eHVwg.jpeg)

- Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.

- Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.

- Ways to orchestrate asynchronous actions in Redux: 
    -  `redux-promise` or `redux-promise-middleware` to dispatch Promises instead of functions.
    - `redux-observable` to dispatch Observables.
    - `redux-saga` middleware to build more complex asynchronous actions.
    - `redux-pack` middleware to dispatch promise-based asynchronous actions.

### Terms

- store: A store holds the whole state tree of your application. It's just an object with a few methods on it.

- combined reducers: The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore .

### Resources

- [Thunk](https://www.digitalocean.com/community/tutorials/redux-redux-thunk)