# Message Queues

**What does it mean that web sockets are bidirectional? Why is this useful?**

- WebSockets allow for full-duplex bidirectional communication, this enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time. Yes it's useful.

**Does socket.io use HTTP? Why?**

- Yes it's use it but it doesn't need an HTTP server to regular websockets,but it is used to allow HTTP and websocket servers to co-exist on the same TCP port.

**What happens when a client emits an event?**

- The event gets passed to the server through websockets. Its a tcp connection from the client to the server. The connection meaning the server can send real time data to the client and vise versa.

**What happens when a server emits an event?**

- It will send an event called message to the client, after the client connects. The send function on socket object associates the 'message' event.

**What happens if a client “misses” an event?**

- The events will be ignored

**How can we mitigate this?**

- You could avoid missing messages by always having the handlers and then deciding in the handlers whether to do anything with the message or not.

**Sockets work based on events. There are some reserved events, which can be accessed using the socket object on the server side.These are :**

1. Connect
2. Message
3. Disconnect
4. Reconnect
5. Ping
6. Join and
7. Leave.

**The client-side socket object also provides us with some reserved events, which are :**

1. Connect
2. Connect_error
3. Connect_timeout
4. Reconnect, etc.

## Terms

- Socket: it was created to use open connections to facilitate realtime communication, still a relatively new phenomenon at the time.

- Web Socket: it is an advanced technology that makes it possible to open a two-way interactive communication session between the user's browser and a server.

- Socket.io: it is a library that enables real-time, bidirectional and event-based communication between the browser and the server.

- Client: a computer hardware device or software that accesses a service made available by a server.

- Server: is a physical computer dedicated to run services to serve the needs of other computers. Depending on the service that is running, it could be a file server, database server, home media server, print server, or web server.

- OSI Model: The Open Systems Interconnection (OSI) model describes seven layers that computer systems use to communicate over a network.

- TCP Model: TCP model defines how devices should transmit data between them and enables communication over networks and large distances. The model represents how data is exchanged and organized over networks.

- TCP: TCP stands for Transmission Control Protocol a communications standard that enables application programs and computing devices to exchange messages over a network.

- UDP: User Datagram Protocol, or UDP, is a communication protocol used across the Internet for especially time-sensitive transmissions such as video playback or DNS lookups.

- Packets: it is a small segment of a larger message.