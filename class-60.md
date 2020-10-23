# Application State with Redux

Redux: A Predictable State Container for JS Apps

- It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. 

- with Redux, it is advisable to store your application state in a single object managed by the Redux store. 

- if you want to update the state of your Redux application (like you do with setState in React), you need to let Redux know about that with an `action`.

- The only way to change the state is to emit an action, an object describing what happened.

- If you want to update the state of your application, you convey your action to the reducer. This process is mostly called dispatching an action.

- Dispatch means sending off the action to the reducers. To specify how the state tree is transformed by actions, you write pure reducers.

- the Redux Reducer is just a function. A function that takes in two parameters. The first being the STATE of the app, and the other the ACTION .

- For a Redux reducer, you always return the new state of your application.

![](https://cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/cbd8cb0f-97ee-4da0-8913-ac9892621c91/redux-example-css-tricks-opt.pg_)

- Testing redux reducers with Jest: Having unit tests for all reducers will prevent any issues related to global application state. It’s especially useful if there are a lot of different API calls and every call will modify a state.

### Terms

- cookies : small items of data, each consisting of a name and a value, stored on behalf of a website by visitors' web browsers.

- authorization : the process of verifying what users have access to.

- access control : selective restriction of access to a resource.

- conditional rendering: Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.


### Resources

-[Guide](https://www.freecodecamp.org/news/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6/)
- [Tutorial](https://egghead.io/courses/getting-started-with-redux)
- [Testing](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)