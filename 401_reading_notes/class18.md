# WebSocket
WebSocket API is an advanced technology that makes it possible to open a 
two-way interactive communication session between the user's browser and a 
server. With this API, you can send messages to a server and receive 
event-driven responses without having to poll the server for a reply.
Websockets allows us to establish a stateful connection between browser 
and server so we can exchange pieces of information in both directions. 
It's more efficient than standard request and response cycle from HTTP.

### WebSocket Drawback
WebSockets are handled differently on different browsers so it's not easy to implement the cross-browser code. And how about older browsers that don't support WebSockets? We need some kind of wrapper that will work on different browsers and fallback to polling techniques on older ones.

# Socket.io
its a tool for creating real-time applications with two-way communication 
between the server-side and the client-side in a syntax that looks as if 
you are just triggering and listening to events. It leverages the power of 
WebSockets along with several fallbacks. It can be used to create 
bidirectional interactions, such as real-time dashboards, chat 
applications, and multiplayer games. **Socket.IO is NOT a WebSocket implementation.** Although Socket.IO indeed uses WebSocket as a transport when possible, it adds some metadata to each packet: the packet type, the namespace and the packet id

## Differences between WebSocket and Socket.IO

The main advantages of Socket.IO over WebSockets are:

* Unlike WebSocket, Socket.IO allows you to broadcast a message to all the connected clients. For instance
* Proxies and load balancers makes WebSockets hard to implement and scale. Socket.IO supports these technologies out of the box.
* Socket.IO is able to fallback to technologies other than WebSockets when the client doesn’t support it.
* If a WebSocket connection drops, it will not automatically reconnect. Socket.IO automatically reconnect
* Socket.IO APIs are built to be easier to work with.



