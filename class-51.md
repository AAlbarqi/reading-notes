# Props and State

![](https://i.stack.imgur.com/wqvF2.png)

- `setState()` is the only legitimate way to update state after the initial state setup.
- The reconciliation process is the way React updates the DOM, by making changes to the component based on the change in state.
- `setState()` should be treated asynchronously — in other words, do not always expect that the state has changed after calling setState().
- You can pass an object or a function to setState()
- Do not depend on this.state immediately after calling setState() and make use of the updater function instead.

Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:
- React events are named using camelCase, rather than lowercase.
- With JSX you pass a function as the event handler, rather than a string.

- f you refer to a method without () after it, such as onClick={this.handleClick}, you should bind that method.
- State is similar to props, but it is private and fully controlled by the component.

- if We want to set up a timer whenever a class is rendered to the DOM for the first time. This is called “mounting” in React. If we want to clear that timer whenever the DOM produced by the calss is removed. This is called “unmounting” in React.
- The componentDidMount() method runs after the component output has been rendered to the DOM. These methods are called “lifecycle methods”.

- In React apps, whether a component is stateful or stateless is considered an implementation detail of the component that may change over time. You can use stateless components inside stateful components, and vice versa.

- Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

- React Testing Library (RTL) is made of simple and complete React DOM testing utilities that encourage good testing practices.

- ARIA defines semantics that can be applied to elements, with these divided into roles (defining a type of user interface element) and states and properties that are supported by a role.

### Discussion

- What does npm run build do?
    - npm run build does nothing unless you specify what "build" does in your package. json file. It lets you perform any necessary building/prep tasks for your project, prior to it being used in another project.
- Why do we prefer to test a React application at the behavior rather than the unit level?
    - Integration tests are a sweet spot between cost and value of tests. Writing integration tests for a React app with the help of react-testing-library instead of or in addition to component unit tests can increase code maintainability without impairing development speed.
- Does a deployed React application require a server?
    - React is a client side UI library. What Node offers is a series of tools that allow you to be able to work with React more easily, such as Webpack (gathers code into a single bundle and listens for file changes to reload this bundle to show the updated code) and Babel (converts ES6 and JSX to plain JavaScript). npx itself is a Node tool which allows you to run a package, in this case with Create React App, which allows you to easily start a new React project. The server that you see is simply to allow for the reloading of the app in response to file changes in real time. The server is only for use in development.

### Term

- BDD : behavior-driven development is an Agile software development process that encourages collaboration among developers, QA and non-technical or business participants in a software project.

- Acceptance Tests : a test conducted to determine if the requirements of a specification or contract are met. 

- mounting : a process by which the operating system makes files and directories on a storage device (such as hard drive, CD-ROM, or network share) available for users to access via the computer's file system.

- build : a version of a program. As a rule, a build is a pre-release version and as such is identified by a build number, rather than by a release number.