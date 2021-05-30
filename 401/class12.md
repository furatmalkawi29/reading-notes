## What is the benefit of transforming data into packets?

Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully


## UDP is often refereed to as a connectionless protocol. Why is this?

No connection needs to be established between the source and destination before you transmit data .

## Can a socket server application have multiple socket connections?

By default, a single server can handle 65,536 socket connections, but we can definitely say that number of WebSocket connections is also limited.

## Can a socket connection application be connected to multiple socket servers?

You can only have one application listening on the same port at one time. Now if you had 2 network cards

## Can an application be both a socket server and a socket connection?

However, if you want to use a client socket and a server socket within a single application, then yes! You can do that if you're willing to use two different ports. Or if the sockets won't be using the same port at the same time.


# Terms

## Observer Pattern

is a design pattern that lets you define a subscription mechanism to notify  about any events that happen to the object they’re observing. 

a real world example is If you subscribe to a newspaper or magazine, you no longer need to go to the store to check if the next issue is available. Instead, the publisher sends new issues directly to your mailbox right after publication or even in advance .


## Listener

listener is programmed to react to an input or signal by calling the event's handler. The term event listener is often specific to Java and JavaScript.


Event Handler

scripts that are automatically executed when an event occurs

Event Driven Programming

is when a program is designed to respond to user engagement in various forms. the flow of program execution is determined by “events.”

Event Loop

has one simple job — to monitor the Call Stack and the Callback Queue. If the Call Stack is empty, the Event Loop will take the first event from the queue and will push it to the Call Stack

Event Queue

repository where application events are held before proccessing . It follows the queue data structure to maintain the correct sequence in which all operations should be sent for execution . 

Call Stack

The call stack is used by JavaScript to keep track of multiple function calls. It is like a real stack in data structures where data can be pushed and popped and follows the Last In First Out (LIFO) principle

Emit/Raise/Trigger

Emitting events: Every event is named event in nodejs. We can trigger an event by emit(event) function


database

A database is an organized collection of data, generally stored and accessed electronically from a computer system. 

<br><br>

# Websocket 

### WebSocket?

communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

<br>

![](https://cdn.educba.com/academy/wp-content/uploads/2018/11/WebSocket-protocol-schema.png)

### Socket.IO?

is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts .

- **Client-Side** : it is the library that runs inside the browser
- **Server Side** : It is the library for Node.js


## note : 

WebSocket is the technology, while Socket.io is a library for WebSockets.


### Key features of Socket.IO

- It helps in broadcasting to multiple sockets at a time and handles the connection transparently.

- It works on all platform, server or device, ensuring equality, reliability, and speed.









