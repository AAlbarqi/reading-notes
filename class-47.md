# TCP Servers

- The Open Systems Interconnection (OSI) model is a conceptual model created by the International Organization for Standardization which enables diverse communication systems to communicate using standard protocols. 

- OSI provides a standard for different computer systems to be able to communicate with each other.

![](https://www.cloudflare.com/img/learning/ddos/what-is-a-ddos-attack/osi-model-7-layers.svg)

- TCP (Transmission Control Protocol) is a standard that defines how to establish and maintain a network conversation through which application programs can exchange data.

- It determines how to break application data into packets that networks can deliver, sends packets to and accepts packets from the network layer, manages flow control and -- because it is meant to provide error-free data transmission -- handles retransmission of dropped or garbled packets and acknowledges all packets that arrive.

- TCP is used for organizing data in a way that ensures the secure transmission between the server and client. It guarantees the integrity of data sent over the network, regardless of the amount. 

![](https://cdn.ttgtmedia.com/rms/onlineImages/networking-osi_vs_tcp-ip_model_table_desktop.jpg)

- The net module provides an asynchronous network API for creating stream-based TCP or IPC servers (net.createServer()) and clients (net.createConnection()).

### Discussion

- Why are events sometimes better than asynchronous actions with callbacks?
    - While the "event handler" pattern is more complex it is much more robust and less likely to hang when an action fails. It also makes for a more responsive GUI. A callback is procedure you pass as an argument to another procedure.

- What does an EventEmitter instance do?
    - All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.

- When is a program’s call stack, event queue, and event loop active?
    - the Event Loop, which keeps running continuously and checks the Main stack, if it has any frames to execute, if not then it checks Callback queue, if Callback queue has codes to execute then it pops the message from it to the Main Stack for the execution.

### Terms : 

- Observer Pattern : a software design pattern in which an object, called the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods. 

- Listener : a procedure in JavaScript that waits for an event to occur.

- Event Handler : scripts that are automatically executed when an event occurs.

- Event Driven Programming : a useful way to create interactive websites. Typically, after the webpage has loaded the JavaScript program continues to run waiting for an event. If you connect this event to a JavaScript function then the function will run when the event occurs.

- Event Loop : It monitors the Call Stack and the Callback Queue. If the Call Stack is empty, it will take the first event from the queue and will push it to the Call Stack, which effectively runs it.

- Event Queue : a data structure similar to the stack — you add items to the back but can only remove them from the front.

- Call Stack : a mechanism for an interpreter, to keep track of its place in a script that calls multiple functions.

- Subscribe : That means it will subscribe itself to the observable of interest (which is getTasks() in your case) and wait until it is successful and then execute the first passed callback function.

- database : an organized collection of structured information, or data, typically stored electronically in a computer system.