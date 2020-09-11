# HTTP and REST

- **HTTP** stands for Hypertext Transfer Protocol.
![](https://cdn.tutsplus.com/net/authors/jeremymcpeak/http1-req-res-details.png)
    - It's a stateless, application-layer protocol for communicating between distributed systems, and is the foundation of the modern web.
    - HTTP allows for communication between a variety of hosts and clients.
    - Communication between a host and a client occurs, via a request/response pair. The client initiates an HTTP request message, which is serviced through a HTTP response message in return.

- **Uniform Resource Locators (URLs)** 
![](https://cdn.tutsplus.com/net/authors/jeremymcpeak/http1-url-structure.png)

URLs reveal the identity of the host which we want to communicate, but the action that should be performed on the host is specified via HTTP verbs: 
    - GET: fetch an existing resource.
    - POST: create a new resource.
    - PUT: update an existing resource.
    - DELETE: delete an existing resource.

- **Status Codes** tells the client how to interpret the server response. types of responses:
    - 1xx: Informational Messages :continue sending the remainder of the request, or ignore if it has already sent it.
    - 2xx: Successful : the request was successfully processed.
        - 202 Accepted.
        - 204 No Content.
        - 205 Reset Content.
        - 206 Partial Content.
    - 3xx: Redirection : This requires the client to take additional action. 
        - 301 Moved Permanently.
        - 303 See Other.
        - 304 Not Modified
    - 4xx: Client Error
        - 400 Bad Request.
        - 401 Unauthorized.
        - 403 Forbidden.
        - 405 Method Not Allowed.
    - 5xx: Server Error
        - 500 Internal Server Error
        - 501 Not Implemented.
        - 503 Service Unavailable.

- **REST** is REpresentational State Transfer. It is architectural style for distributed hypermedia systems.
- an architectural style and approach to communications often used in web services development. 
- A RESTful API is an application program interface (API) that uses HTTP requests to GET, PUT, POST and DELETE data.
## Discussion 

1. Name 3 cloud based NoSQL Databases
    - mongodb
    - Oracle NoSQL Database
    - HBase
2. What is the advantage of an ORM, like Mongoose?
    - ORMs will shield applications from SQL injection attacks since the framework will filter the data. ORMs provide the concept of Database Abstraction which makes switching databases easier and creates a consistent code base for the application
3. How does the repository pattern compare with an ORM?
    - THe ORM is an implementation detail of the Repository. The ORM just makes it easy to access the db tables in an OOP friendly way. That's it.
4. When making a repository/facade, what flexibility do you gain?
    - A facade can make a software library easier to use, understand and test, since the facade has convenient methods for common tasks. - make the library more readable, for the same reason.


## Term

- lifecycle : Application lifecycle is a key way that modern OSs manage resources.

- collections : a form of memory management whereby objects that are no longer referenced are automatically deleted and their resources are reclaimed.

- the “Repository” design pattern : a kind of container where data access logic is stored. 

- mongoose middleware : functions that can intercept the process of the init, validate, save, and remove instance methods.

- Object Relation Mapping (ORM) : a programming technique for converting data between incompatible type systems using object-oriented programming languages.

### Resouces:
[HTTP](https://code.tutsplus.com/tutorials/http-the-protocol-every-web-developer-must-know-part-1--net-31177)