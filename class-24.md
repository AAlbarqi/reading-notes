# THE CALL STACK

A **call stack** is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

![](https://res.cloudinary.com/practicaldev/image/fetch/s--c6u1ewY3--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://res.cloudinary.com/practicaldev/image/fetch/s--dM0jXped--/c_imagga_scale%2Cf_auto%2Cfl_progressive%2Ch_420%2Cq_auto%2Cw_1000/https://dev-to-uploads.s3.amazonaws.com/i/agxpgg948lpni5rs5kos.png)

In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.

At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

- **Manage function invocation (call)** : The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.

- **A stack overflow** occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

The key takeaways from the call stack are:
1. It is single-threaded. Meaning it can only do one thing at a time.
2. Code execution is synchronous.
3. A function invocation creates a stack frame that occupies a temporary memory.
4. It works as a LIFO — Last In, First Out data structure.

#### JavaScript error messages & debugging

###### Types of error messages
1. Reference errors
When you try to use a variable that is not yet declared you get this type os errors.
   - `console.log(foo) // Uncaught ReferenceError: foo is not defined`
**the fix** is as simple has declaring the variable before any declaration is made.
2. Syntax errors
this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
   - `JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1`
**the fix** This can be solved by just fixing the syntax
3. Range errors
   - `var foo= [];`
     `foo.length = foo.length -1 // Uncaught RangeError: Invalid array length`
4. Type errors
this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
   - `var foo = {}`
     `foo.bar // undefined`
     `foo.bar.baz // Uncaught TypeError: Cannot read property 'baz' of undefined`
**The fix**, just make sure that bar exists before trying to access it, either by creating bar or by checking for undefined.

##### Debugging
To debug your JS code, the easiest and maybe the most common way its to simply console.log() the variables you want to check or, by using chrome developer tools, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again (F5).
![](https://developers.google.com/web/tools/chrome-devtools/javascript/imgs/sources.png)
