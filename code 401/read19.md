#### What does it mean that web sockets ? 
* Why is this useful? This mean that the connection is directly between the client and the server use TCP no HTTP. Bcause you don't need to handle every request from client you just use events

What happens when a client emits an event? 
* The server take that emit message and the paylod and resopond with and action or another emit message.

What happens when a server emits an event? 
- The client take this emit and respond to it with an action or another emit messages.

What happens if a client “misses” an event? 
- nothing actually that mean the event never been triggered the app will still functions the right way.

How can we mitigate this?? 
- you can avoid missing events by having a handler for each event that take an action.

Does socket.io use HTTP? 
- Why? No, it use a TCP connection. Because the TCP allow for direct connection between the client and the server on the other hand HTTP deal with request and resoponse which will not useful for events.

Vocabulary
Socket: is a library that enables real-time,  event-based communication between the browser and the server.

Websocket: WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

Client: A Web client typically refers to the Web browser in the user's machine or mobile device.

Server: It's a computer program that distributes web pages as they are requisitioned.
* The basic objective of the web server is to store, process and deliver web pages to the users

OSI Model: The Open Systems Interconnection (OSI) model describes seven layers that computer systems use to communicate over a network.

TCP/IP: stands for Transmission Control Protocol/ Internet Protocol. It is specifically designed as a model to offer highly reliable and end-to-end byte stream over an unreliable internetwork..

TCP: Transmission Control Protocol (TCP) is a communications standard that enables application programs and computing devices to exchange messages over a network. It is designed to send packets across the internet and ensure the successful delivery of data and messages over networks.

UDP: User Datagram Protocol (UDP) – a communications protocol that facilitates the exchange of messages between computing devices in a network. It's an alternative to the transmission control protocol (TCP).

Packet: is a small amount of data sent over a network, such as a LAN or the Internet. Similar to a real-life package, each packet includes a source and destination as well as the content (or data) being transferred.

