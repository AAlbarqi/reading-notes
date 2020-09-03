# Node Ecosystem, TDD, CI/CD

![](https://www.hugeserver.com/kb/wp-content/uploads/2017/03/1_hj-_anuWthYZs0x22hE9lA-e1520240360455.png)

- What is Node.js?
    1. Node.js is an open source server environment
    2. Node.js runs on various platforms (Windows, Linux, Unix, Mac OS X, etc.)
    3. Node.js uses JavaScript on the server

- What Can Node.js Do?
    1. Node.js can generate dynamic page content
    2. Node.js can create, open, read, write, delete, and close files on the server
    3. Node.js can collect form data
    4. Node.js can add, delete, modify data in your database

- What is a Node.js File?
    1. Node.js files contain tasks that will be executed on certain events
    2. A typical event is someone trying to access a port on the server
    3. Node.js files must be initiated on the server before having any effect
    4. Node.js files have extension ".js"

#### npm

npm is the world’s largest software registry. Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well.

npm consists of three distinct components:
1. the website
2. the Command Line Interface (CLI)
3. the registry

Use the website to discover packages, set up profiles, and manage other aspects of your npm experience. For example, you can set up Orgs (organizations) to manage access to public or private packages.

The CLI runs from a terminal, and is how most developers interact with npm.

The registry is a large public database of JavaScript software and the meta-information surrounding it.

#### Array.map()

The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.

#### Array.reduce()

The reduce() method reduces the array to a single value. It executes a provided function for each value of the array (from left-to-right). The return value of the function is stored in an accumulator (result/total).

#### How to use superagent() to fetch data from a URL and log the result:
1. With normal Promise .then() syntax:

`superagent.get(URL)
    .then(data => {
        console.log(data.body);
    }).catch(err => console.error(err))`
  
2. with async / await syntax:

`async function getCity(city){
  try{
  let result = await superagent.get(URL);
  console.log(result.body);
  } catch(e) {console.error(e)};
}`

#### Promises

The Promise object represents the eventual completion (or failure) of an asynchronous operation, and its resulting value.

**Question** : Are all callback functions considered to be Asynchronous? Why or Why Not?
No. Only I/O is usually asynchronous, but many other callbacks are synchronous. 
Simply taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous. 