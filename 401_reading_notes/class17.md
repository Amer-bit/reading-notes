# TCP Servers
TCP/IP stands for Transmission Control Protocol/ Internet Protocol. It is specifically designed as a model to offer highly reliable and end-to-end byte stream over an unreliable internetwork.

## TCP Characteristics
the essential characteristics of TCP/IP protocol

* Support for a flexible architecture
* Adding more system to a network is easy.
* In TCP/IP, the network remains intact until the source, and destination machines were functioning properly.
* TCP is a connection-oriented protocol.
* TCP offers reliability and ensures that data which arrives out of sequence should put back into order.
* TCP allows you to implement flow control, so sender never overpowers a receiver with data.

![TCP/IP Conceptual Layers](https://www.guru99.com/images/1/093019_0615_TCPIPModelW1.png)

The functionality of the TCP/IP model is divided into four layers, and each includes specific protocols.

TCP/IP is a layered server architecture system in which each layer is defined according to a specific function to perform. All these four layers work collaboratively to transmit the data from one layer to another.

* Application Layer
* Transport Layer
* Internet Layer
* Network Interface

### Application Layer
Application layer interacts with an application program, which is the highest level of OSI model this is what the user interacts with, such as email and messaging. The application layer is the OSI layer, which is closest to the end-user. It means the OSI application layer allows users to interact with other software application.

**The function of the Application Layers are:**

* Application-layer helps you to identify communication partners, determining resource availability, and synchronizing communication.
* It allows users to log on to a remote host
* This layer provides various e-mail services
* This application offers distributed database sources and access for global information about various objects and services.

### Transport Layer
It determines how much data should be sent where and at what rate. This layer builds on the message which are received from the application layer. It helps ensure that data units are delivered error-free and in sequence.

**Important functions of Transport Layers:**

* It divides the message received from the session layer into segments and numbers them to make a sequence.
* Transport layer makes sure that the message is delivered to the correct process on the destination machine.
* It also makes sure that the entire message arrives without any error else it should be retransmitted.

### Internet Layer
The main work of this layer is to send the packets from any network, and any computer still they reach the destination irrespective of the route they take.


## Differences between OSI and TCP/IP Models

![OSI and TCP/IP Models](https://www.guru99.com/images/1/093019_0615_TCPIPModelW3.png)


## Most Common TCP/IP Protocols

* TCP
* IP
* HTTP
* FTP
* DNS