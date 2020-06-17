# Message Queues
A **queue** is a line of things waiting to be handled, starting at the beginning of the line and processing it in sequential order. A message queue is a queue of messages sent between applications. It includes a sequence of work objects that are waiting to be processed.

A **message** is the data transported between the sender and the receiver application; it's essentially a byte array with some headers at the top. An example of a message could be something that tells one system to start processing a task, it could contain information about a finished task or just be a plain message.

The **basic architecture of a message queue** is there are **client** applications called **producers** that create messages and deliver them to the message queue. Another application, called a **consumer**, connects to the queue and gets the messages to be processed. Messages placed onto the queue are stored until the consumer retrieves them.


A **message queue** provides an **asynchronous communications protocol**, which is a system that puts a message onto a message queue and does not require an immediate response to continuing processing. Email is the best example of asynchronous communication. When an email is sent, the sender continues to process other things without needing an immediate response from the receiver. This way of handling messages decouples the producer from the consumer so that they do not need to interact with the message queue at the same time.

# Socket.io Namespaces
Socket.IO allows you to “namespace” your sockets, which essentially means assigning different endpoints or paths.

This is a useful feature to minimize the number of resources (TCP connections) and at the same time separate concerns within your application by introducing separation between communication channels.

**Default namespace**

We call the default namespace / and it’s the one Socket.IO clients connect to by default, and the one the server listens to by default.


**Custom namespaces**

To set up a custom namespace, you can call the of function on the server-side

### Rooms
Within each namespace, you can also define arbitrary channels that sockets can join and leave.

We can call join to subscribe the socket to a given channel:

`io.on('connection', function(socket){`
  `socket.join('some room')`;
`});`
And then simply use to or in (they are the same) when broadcasting or emitting:

`io.to('some room').emit('some event');`

To leave a channel you call leave in the same fashion as join. Both methods are asynchronous and accept a callback argument.