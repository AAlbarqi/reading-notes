# Event Driven Applications

- Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

- Event-Driven Programming makes use of the following concepts:

    - An Event Handler is a callback function that will be called when an event is triggered.
    - A Main Loop listens for event triggers and calls the associated event handler for that event.

- Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away.

![](https://upload.wikimedia.org/wikipedia/commons/c/cb/Event_driven_programming_Simply_Explained.jpg)

- Much of the Node.js apps are built around an asynchronous event-driven architecture in which certain kinds of objects (called "emitters") emit named events that cause Function objects ("listeners") to be called.

- The EventEmitter calls all listeners synchronously in the order in which they were registered.


### Discussion

1. Why is access control important?
    - to minimize the risk of unauthorized access to physical and logical systems.

2. What is a role used for?
    - A role defines a set of users and/or servers.

3. Why is role based access control more scalable than discretionary or mandatory access control?
    - Because mandatory access control doesn’t scale automatically.

### Terms

- Authorization : is a security mechanism used to determine user/client privileges or access levels related to system resources, including computer programs, files, services, data and application features.

- Role Based Access Control : is an approach to restricting system access to authorized users. 

- Capabilities : is a communicable, unforgeable token of authority. It refers to a value that references an object along with an associated set of access rights.
