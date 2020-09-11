# API Server

![](https://www.cdata.com/apiserver/img/apiserver.png)

- router.param(name, callback):
The parameters of the callback function are:

    - req, the request object.
    - res, the response object.
    - next, indicating the next middleware function.
    - The value of the name parameter.
    - The name of the parameter.

- Unlike app.param(), router.param() does not accept an array of route parameters.

- **Mongoose** has 4 types of middleware: document middleware, model middleware, aggregate middleware, and query middleware. Document middleware is supported for the following document functions. In document middleware functions, this refers to the document.

- **Subdocuments** are documents embedded in other documents. In Mongoose, this means you can nest schemas in other schemas. Mongoose has two distinct notions of subdocuments: arrays of subdocuments and single nested subdocuments.

- **Populate Virtuals** arrays that grow without bound are a MongoDB anti-pattern. Using mongoose virtuals, you can define more sophisticated relationships between documents.

## Discussion

1. How does route prefixing work with an external routing module? by importing and exporting, a group of routes may be prefixed by using the prefix option in the attributes array of a group
2. When routing, what’s the difference between app.get('/data/:id') and app.get('/data/:name')? when the req will be processed the params name and id will be different.
3. Explain how Express handles routing conflicts? override the last one of the conflicts routes.
4. What are the ways that a browser can send “data” or request variables to an HTTP server? POST and PUT is used to send data to a server to create/update a resource.

## Terms

- Routing : refers to how an application’s endpoints (URIs) respond to client requests.
- Route Prefixing : Route grouping is a concept to make the route function that receive same prefix of different requests.
- Request “Body” : data sent by the client to your API
- Request “Query” : QueryString is a collection used to retrieve the variable values in the HTTP query string
- Request “Params” : a combination of the keys/values you'll find in Request.Querystring , Request.Form , Request.Cookies , Request.ServerVariables