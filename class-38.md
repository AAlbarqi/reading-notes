# Express Routing & Connected API

- **Routing** refers to how an application’s endpoints (URIs) respond to client requests.

- **Route methods** : A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.

- There is a special routing method, app.all(), used to load middleware functions at a path for all HTTP request methods. 

![](https://miro.medium.com/max/1042/1*uwNmNlj_t6NSVLULu3R5ug.png)

we can:

1. Use express.Router() multiple times to define groups of routes
2. Apply the express.Router() to a section of our site using app.use()
3. Use route middleware to process requests
4. Use route middleware to validate parameters using .param()
5. Use app.route() as a shortcut to the Router to define multiple requests on a route

## Discussion

1. True or false: The route handler is middleware? somtimes yes sometimes No
2. In what ways can a middleware function end the process and send data to the browser? by calling res.end, res.send, res.render or any method that implicitely calls res.end
3. At what point in the request lifecycle can you “inject” middleware? before the start of the request lifecycle.
4. What can cause express to error with “Request headers sent twice, cannot start a second response”? when a reponse or some callbacks are called twice.

## Terms

- Middleware : functions that have access to the request object (req), the response object (res), and the next middleware function in the - application’s request-response cycle.

- Request Object : what retrieves the values that the client browser passed to the server during an HTTP request.

- Response Object : communicates between the server and the output which is sent to the client.

- Application Middleware : software that provides services beyond those provided by the operating system to enable the various components of a distributed system to communicate and manage data.

- Routing Middleware : determining how an application responds to a client request to a particular endpoint.