## Why is access control important?
control is important because it is a valuable security technique that can be used to regulate who or what can view or use any given resource. ... Without proper access control you could leave your staff and your company wide open to problems such as data loss, theft or breach of privacy and data protection laws.


## Describe an application that would need access control.
the system of university where the student can enroll course and the teacher can create course but the studen can not


## What is a role used for?
To add the privilages for each user that he allowed to do.


*  An **authorization** is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space.

* **role-based access control (RBAC)** is an approach to restricting system access to authorized users.

* A **capability** describes a transferable right to perform one (or more) operations on a given object. It can be obtained by the following combination: An unforgeable reference (in the sense of object references or protected pointers) that can be sent in messages.



# Event Driven Programming 

- Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision. In this article we’re going to go over how Event-Driven Programming works and how we can make the best use of it in our Node.js projects


- Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a click event is triggered. When you press a key a keydown event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.

- We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.

- The eventEmitter.emit() method allows an arbitrary set of arguments to be passed to the listener functions. Keep in mind that when an ordinary listener function is called, the standard this keyword is intentionally set to reference the EventEmitter instance to which the listener is attached.


- All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.



- asynchronous event-driven architecture in which certain kinds of objects (called "emitters") emit named events that cause Function objects ("listeners") to be called.


- The EventEmitter calls all listeners synchronously in the order in which they were registered. This ensures the proper sequencing of events and helps avoid race conditions and logic errors. When appropriate, listener functions can switch to an asynchronous mode of operation using the setImmediate() or process.nextTick()