# Classes, Inheritance, Functional Programming

#### TDD

Test-Driven Development in JavaScript, (TDD) is a technique for ensuring that your code does what you think it does.

#### Inheritance and the prototype chain

- Setting a property to an object creates an own property. The only exception to the getting and setting behavior rules is when there is an inherited property with a getter or a setter.
An inherited function acts just as any other property.
- When an inherited function is executed, the value of this points to the inheriting object, not to the prototype object where the function is an own property.

#### This

-A property of an execution context (global, function or eval) that, in non–strict mode, is always a reference to an object and in strict mode can be any value.

- The value of this is determined by how a function is called (runtime binding). It can't be set by assignment during execution, and it may be different each time the function is called. 

-  `bind()` method to set the value of a function's this regardless of how it's called.

#### Classes

- Classes are in fact "special functions", and just as you can define function expressions and function declarations, the class syntax has two components: class expressions and class declarations.

**Note** : An important difference between function declarations and class declarations is that function declarations are hoisted and class declarations are not. You first need to declare your class and then access it.

#### Discussion

- Why would you want to run JavaScript code outside of a browser?
    - Running JavaScript inside a browser means you are interacting with Web UI (HTML and CSS components) which is displayed on a user's screen. Running JavaScript without/outside a browser means you are using node. js technology to execute your JavaScript code.

- What is the difference between a module and a package?
    - A module is a single file (or files) that are imported under one import and used. e.g. A package is a collection of modules in directories that give a package hierarchy.

- What does the node package manager do?
    - Node Package Manager (NPM) is a command line tool that installs, updates or uninstalls Node. js packages in your application. It is also an online repository for open-source Node.

- 3 different ways to export a function from a node module.
    - `exports.getName = getName;`
    - `exports.getName = () => { return 'Jim'; };`
    - `module.exports = getName;`

#### Terms

- **Ecosystem** The JavaScript ecosystem is a collection of software packages, libraries, and other resources that facilitate development as they integrate with each other.

- **Node.js®** is a JavaScript runtime built on Chrome's V8 JavaScript engine.

- **V8 JavaScript engine** is Google's open source high-performance JavaScript and WebAssembly engine, written in C++. It is used in Chrome and in Node. js, among others.

- **module** (“ES modules” or “ECMAScript modules”) are a major new feature, or rather a collection of new features.

- **A package** is one or more modules (libraries) grouped (or packaged) together.

- **node package manager** is a command line tool that installs, updates or uninstalls Node. js packages in your application. It is also an online repository for open-source Node. js packages.

- **Server** (Server Side JavaScript (SSJS)) is an extended version of JavaScript that enables back-end access to databases, file systems, and servers. javascript code running over a server local resources.

- **environment** gives you support for file access, network access, database access etc.

- **Interpreter** is a program that executes instructions written in a high-level language.

- **A compiler** is a special program that processes statements written in a particular programming language and turns them into machine language or "code" that a computer's processor uses. 
