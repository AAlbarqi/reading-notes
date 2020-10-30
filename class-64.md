# React Native

- React Native is an open-source mobile application framework created by Facebook, it uses native components instead of web components as building blocks.

- Two main components we import from react-native.The Text component allows us to render a text, while the View component renders a container.(A View is useful as a container for other components, to help control style and layout,like div and span).

- Props: Parameters used to customize components when they are created.

- State allows React components to change their output over time in response to user actions, network responses and anything else.

- the difference between state and props in React?
In a React component, the props are the variables that we pass from a parent component to a child component. Similarly, the state are also variables, with the difference that they are not passed as parameters, but rather that the component initializes and manages them internally.

![](https://reactnative.dev/docs/assets/diagram_ios-android-views.svg)

- Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.

![](https://res.cloudinary.com/practicaldev/image/fetch/s--IkN6Jkfv--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://i.imgur.com/wIVQJjm.png)

- ExpoKit is an Objective-C and Java library that allows you to use the Expo platform and your existing Expo project as part of a larger standard native project.

### Terms

- redux toolkit slices: an object of reducer functions, a slice name, and an initial state value and lets us auto-generate action types and action creators, based on the names of the reducer functions that we supply.

- namespace: a set of signs (names) that are used to identify and refer to objects of various kinds.