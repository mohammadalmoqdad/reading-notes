
## What is the benefit of transforming data into packets?
- to avoid using big cables to transform it

## UDP is often refereed to as a connectionless protocol. Why is this?
- UDP is often refereed to as a connectionless protocol. Why is this?

## Can a socket server application have multiple socket connections?
- yes

## Can a socket connection application be connected to multiple socket servers?
- no







# WebSocket 
- DEF: is a computer communications protocol, providing full-duplex communication channels over a single TCP connection

- The WebSocket protocol enables interaction between a web browser (or other client application) and a web server with lower overhead than half-duplex alternatives such as HTTP polling, facilitating real-time data transfer from and to the server.
- This is made possible by providing a standardized way for the server to send content to the client without being first requested by the client, and allowing messages to be passed back and forth while keeping the connection open.

- Unlike HTTP, WebSocket provides full-duplex communication. Additionally, WebSocket enables streams of messages on top of TCP.


 * **Socket.IO** is a library which enables real-time and full duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts, both WebSocket vs Socket.io are event-driven libraries: 
   1. Client Side: it is the library that runs inside the browser
   2. Server Side: It is the library for Node.js


- Why do we need WebSocket?
It provides the full duplex communication which helps in persisting the connection established between the Client and the Web Server.
It also lives up to the standards and provides the accuracy and efficiency stream events to and from with negligible latency.
WebSocket removes the overhead and reduce complexity.
It makes real-time communication effortless and efficient.


