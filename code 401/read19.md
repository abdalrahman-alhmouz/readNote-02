#### What does it mean that web sockets ? 
* Why is this useful?
*  This mean that the connection is directly between the client and the server use TCP no HTTP. 
*  Bcause you don't need to handle every request from client you just use events



What happens when a server emits an event? 
- The client take this emit and respond to it with an action or another emit messages.



Does socket.io use HTTP? 
- Why? No, it use a TCP connection. Because the TCP allow for direct connection between the client and the server on the other hand HTTP deal with request and resoponse which will not useful for events.

Socket: is a library that enables real-time,  event-based communication between the browser and the server.

Websocket: WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

Client: A Web client typically refers to the Web browser in the user's machine or mobile device.

Server: It's a computer program that distributes web pages as they are requisitioned.
* The basic objective of the web server is to store, process and deliver web pages to the users

![socket](https://www.fullstackpython.com/img/visuals/websockets-flow-with-client-push.png)
