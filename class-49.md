# Message Queues

- Sockets have traditionally been the solution around which most real-time chat systems are architected, providing a bi-directional communication channel between a client and a server.

- Within each Namespace, you can define arbitrary channels called “Rooms” that sockets can join and leave.

This is useful to broadcast data to a subset of sockets:

![](https://socket.io/images/rooms.png)
### Terms :

- Web Socket : a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

- Socket.io : a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. 

- Client : a computer or a program that, as part of its operation, relies on sending a request to another program or a computer hardware or software that accesses a service made available by a server (which may or may not be located on another computer).

- Server : a piece of computer hardware or software (computer program) that provides functionality for other programs or devices, called "clients".

### Resources

[cheatsheet](https://socket.io/docs/emit-cheatsheet/)