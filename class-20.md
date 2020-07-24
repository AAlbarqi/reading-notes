# Node Express and Apis

- Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.
- Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.
- Node.js is a program we can use to execute JavaScript on our computers. In other words, it’s a JavaScript runtime.

##### npm, the JavaScript Package Manager

Node comes bundled with a package manager called npm.
npm is also the world’s largest software registry.
- To check which version you have installed on your system, type `npm -v`.

##### Working with the package.json File
node_modules. This is where npm has saved lodash and any libraries that lodash depends on. The node_modules folder shouldn’t be checked in to version control, and can, in fact, be re-created at any time by running npm install from within the project’s root.

##### What Is Node.js Used For?

- installing (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.

- They can be used for anything from bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking.

##### The Node.js Execution Model

It’s also event-driven, which means that everything that happens in Node is in reaction to an event. For example, when a new request comes in (one kind of event) the server will start processing it. If it then encounters a blocking I/O operation, instead of waiting for this to complete, it will register a callback before continuing to process the next event. When the I/O operation has finished (another kind of event), the server will execute the callback and continue working on the original request.

- The following image depicts Node’s execution model:

![](https://dab1nmslvvntp.cloudfront.net/wp-content/uploads/2012/10/1516152673node_event_loop.png)

##### Downsides

- The fact that Node runs in a single thread does impose some limitations. For example, blocking I/O calls should be avoided, CPU-intensive operations should be handed off to a worker thread, and errors should always be handled correctly for fear of crashing the entire process.


#### Example
- `const http = require('http');`
- requiring Node’s native HTTP module.
- `http.createServer((request, response) => { //the request from the user and the response, which we use to send back a 200 HTTP status code, along with our “Hello World!” message.
  response.writeHead(200);
  response.end('Hello, World!');
}).listen(3000);` 
- createServer method to create a new web server object, to which we pass an anonymous function
- This function will be invoked for every new connection that’s made to the server.
- Finally, we tell the server to listen for incoming requests on port 3000, and output a message to the terminal to let us know it’s running.
console.log('Server running on http://localhost:3000');`

##### What Kind of Apps Is Node.js Suited To?

- Node is particularly suited to building applications that require some form of **real-time interaction** or collaboration — for example, chat sites, or apps such as CodeShare, where you can watch a document being edited live by someone else.
- It’s also a good fit for **building APIs** where you’re handling lots of requests that are I/O driven (such as those needing to perform operations on a database), or for sites involving **data streaming**, as Node makes it possible to process files while they’re still being uploaded.

##### The Advantages of Node.js
1. speed and scalability
2. you can easily share code between the server and the client.
3. it speaks JSON.
4. transitioning to Node development is potentially easier than to other server-side languages.
5.  it can be used as a scripting language to automate repetitive or error prone tasks on your PC
6. Node.js can also can be used to build cross-platform desktop apps and even to create your own robots. 



