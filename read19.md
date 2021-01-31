


## What does it mean that web sockets are bidirectional? Why is this useful?
it means it can send and receive at the same time which allow the synchronous connection


## Does socket.io use HTTP? Why?
no, because it is one direction protocol

## What happens when a client emits an event?
the payload inside is broadcasted to all clients


* The WebSocket API is an advanced technology that makes it possible to open a two-way interactive communication session between the user's browser and a server. With this API, you can send messages to a server and receive event-driven responses without having to poll the server
* Socket.IO enables real-time bidirectional event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed. Socket.IO is built on top of the WebSockets API (Client side) and Node. js. It is one of the most depended upon library on npm (Node Package Manager).
* client is a computer or a program that, as part of its operation, relies on sending a request to another program or a computer hardware or software that accesses a service made available by a server (which may or may not be located on another computer)
* “server” is a web application server at a remote location that will process web requests and send pages to the client. Web applications can contain code that is processed on the client's browser or on the web server





- The following events are reserved and should not be used as event names by your application:
connect
connect_error
disconnect
disconnecting
newListener
removeListener
 Default room

- Each Socket in Socket.IO is identified by a random, unguessable, unique identifier Socket#id. For your convenience, each socket automatically joins a room identified by its own id.
 rooms are a server-only concept (i.e. the client does not have access to the list of rooms it has joined).
 Rooms

- A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients