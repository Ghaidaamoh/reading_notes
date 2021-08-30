# Socket.io

**What Socket.IO is**

- Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server. It consists of:

  - a Node.js server: Source|API
  - a Javascript client library for the browser (which can be also run from Node.js): Source|API

**What is the benefit of transforming data into packets?**

- TDM-based networks must transform into packet-based networks to meet the demands of pervasive data-centric applications and services.

- Packet-based networks not only enable new innovations, services, and business opportunities, they are also the most cost-effective, efficient, and scalable networks for content delivery.

**UDP is often refereed to as a connectionless protocol. Why is this?**

- Because it is analogous to sending a letter where you don't acknowledge receipt.

**Can a socket server application have multiple socket connections?**

- Yes, Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.

**Can a socket connection application be connected to multiple socket servers?**

- No,a server socket listens on a single port. All established client connections on that server are associated with that same listening port on the server side of the connection.

**Can an application be both a socket server and a socket connection?**

- No, You can not combine server and client sockets into one, because a TCP/IP connection goes from a source port to a destination port, with each having unique port numbers.

## Terms

- Observer Pattern: is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

- Listener: It is a JavaScript function which respond to the event occur.

- Event Handler: which is a block of code usually a JavaScript function that you as a programmer create that runs when the event fires.

- Event Driven Programming: is a programming paradigm in which the flow of the program is determined by events such as user actions mouse clicks, key presses, sensor outputs, or message passing from other programs or threads.

- Event Loop: is the secret behind JavaScript’s asynchronous programming. JS executes all operations on a single thread, but using a few smart data structures, it gives us the illusion of multi-threading.

- Event Queue: is responsible for sending new functions to the track for processing. It follows the queue data structure to maintain the correct sequence in which all operations should be sent for execution.

- Call Stack: is responsible for keeping track of all the operations in line to be executed. Whenever a function is finished, it is popped from the stack.

- Emit/Raise/Trigger: method is used to trigger the event.

- Subscribe: The .subscribe() function is similar to the Promise.then(), .catch() and .finally() methods, but instead of dealing with promises it deals with Observables.

- database: it's implements a common, promise-based interface for SQL database access. Inspired by Java, it uses connection strings to identify the database driver. Wrappers around native database drivers provide a unified interface to handle databases