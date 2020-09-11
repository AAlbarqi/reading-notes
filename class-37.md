# Express

- Express is a routing and middleware web framework that has minimal functionality of its own: An Express application is essentially a series of middleware function calls.

- Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle.

Middleware functions can perform the following tasks:

1. Execute any code.
2. Make changes to the request and the response objects.
3. End the request-response cycle.
4. Call the next middleware function in the stack.

**Routing** refers to how an application’s endpoints (URIs) respond to client requests.

![](https://www.tutorialspoint.com/expressjs/images/middleware_desc.jpg)

## Discussion

1. What’s the difference between PUT and PATCH?
    - the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server
    - MockServer, Beeceptor, Mockoon, Mocky.io

3. Compare and contrast SOAP and ReST
    - SOAP stands for Simple Object Access Protocol whereas REST stands for Representational State Transfer. SOAP is a protocol whereas REST is an architectural pattern

## Terms

- SOAP : Simple Object Access Protocol.

- ReST Verbs : POST, GET, PUT, PATCH, and DELETE

- CRUD Verbs : create, read, update, and delete

- Swagger : a set of rules (in other words, a specification) for a format describing REST APIs, that help us document our APIs.