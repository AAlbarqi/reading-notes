# JS Debugging

When an Error object is created, it will contain the following properties:

| PROPERTY | DESCRIPTION |
| ------------- | ------------- |
| name | Type of execution |
| message | Description |
| fileNumber | Name of the JavaScript file |
| lineNumber | Line number of error |

There are seven types of built-in error objects in JavaScript. You'll see them on the next two pages:

| OBJECT | DESCRIPTION |
| ------------- | ------------- |
| Error | Generic error - the other errors are all based upon this error |
| Syntax Error | Syntax has not been followed |
| ReferenceError | Tried to reference a variable that is not declared/within scope|
| TypeError | An unexpected data type that
cannot be coerced |
| Range Error | Numbers not in acceptable range |
| URI Error | encodeURI ().decodeURI(),and
similar methods used incorrectly |
| EvalError | eval () function used incorrectly |

#### HOW TO DEAL WITH ERRORS?
1. DEBUG THE SCRIPT TO FIX ERRORS 
2. HANDLE ERRORS GRACEFULLY 

- **Debugging** is about deduction: eliminating potential causes of an error.

#### BROWSER DEV TOOLS & JAVASCRIPT CONSOLE 
CHROME/ OPERA :On a PC, press the F12 key or:
1. Go to the options menu (or three line menu icon)
2. Select Toots or More tools.
3. Select JavaScript Console or Developer Tools On a Mac press Alt + Cmd + J. Or:
4. Go to the View menu.
5. Select Developer.
6. Open the JavaScript Console or Developer Tools option and select Console. 

#### CONSOLE METHODS
1. console. info() can be used for general information
2. console.warn() can be used for warnings
3. console.error() can be used to hold errors

**Note** : You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time. 

![](https://developers.google.com/web/tools/chrome-devtools/javascript/imgs/sources-annotated.png)

#### HANDLING EXCEPTIONS 

`try {// Try to execute this code}`
`catch (exception) {//If there is an exception, run this code}`
`finally {// This always gets executed }`

#### THROWING ERRORS
- If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback. 
`throw new Error('message'); `

 