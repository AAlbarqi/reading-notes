# Redux - Combined Reducers

- reducers (Object): An object whose values correspond to different reducing functions that need to be combined into one. 

- Returns a function: A reducer that invokes every reducer inside the reducers object, and constructs a state object with the same shape.

- `combineReducers(reducers)` : The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

- The resulting reducer calls every child reducer, and gathers their results into a single state object.

- The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers()

- You can control state key names by using different keys for the reducers in the passed object. For example, you may call `combineReducers({ todos: myTodosReducer, counter: myCounterReducer })` for the state shape to be `{ todos, counter }`.

- Any reducer passed to combineReducers must satisfy the following rules:

    - For any action that is not recognized, it must return the state given to it as the first argument.

    - It must never return undefined. 

    - If the state given to it is undefined, it must return the initial state for this specific reducer, the initial state must not be undefined either.

![](https://krasimirtsonev.com/blog/article/my-take-on-redux-architecture/assets/redux-reallife.jpg)

### Terms
- immutable state: An immutable value or object cannot be changed, so every update creates new value, leaving the old one untouched.

- time travel in redux: the ability step forward and backward through the state of you application.

- action creator: a function that returns an action object.

- reducer: a pure function that takes the previous state and an action, and returns the next state. 

- dispatch: a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change.

### Resources