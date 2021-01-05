
## Name 3 real world use cases where you’d want to change the request with custom middleware
1. Data Access. Database access services.
2. Transactions. Platforms for executing business transactions such as market trades.
3. Integration. Tools for data or process integration such as an enterprise service bus.


## True or false: The route handler is middleware?
- false

## In what ways can a middleware function end the process and send data to the browser?
- using `next()` function 

## At what point in the request lifecycle can you “inject” middleware?
- after too runing time being caused.

## What can cause express to error with “Request headers sent twice, cannot start a second response”
- When you see this error, try to look for anything that tries to send a header after some of the body has already been written. For example, look for callbacks that are accidentally called twice, or any error that happens after the body is sent.


* **Middleware** is software that provides common services and capabilities to applications outside of what's offered by the operating system.

* **The Request object** retrieves the values that the client browser passed to the server during an HTTP request

*  **Response object** is the object which communicates between the server and the output which is sent to the client.

* **Middleware application** is software which lies between an operating system and the applications running on it. This can include security authentication, transaction management, message queues, applications servers, web servers and directories.

* **Routing Middleware** is the process of selecting a path for traffic in a network or between or across multiple networks.









