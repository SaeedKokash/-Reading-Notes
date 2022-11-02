# Readings: Socket BE #

## OSL Model ##

### What is the OSI model ###
The OSI model is a conceptual framework that is used to describe how a network functions. In plain English, the OSI model helped standardize the way computer systems send information to each other.

### Nodes ###
A node is a physical electronic device hooked up to a network, for example a computer, printer, router, and so on. If set up properly, a node is capable of sending and/or receiving information over a network.

![image](https://www.freecodecamp.org/news/content/images/size/w1000/2021/11/1-Router-Image.jpeg)

### Links ###
Links connect nodes on a network. Links can be wired, like Ethernet, or cable-free, like WiFi.

### Protocol ###
A protocol is a mutually agreed upon set of rules that allows two nodes on a network to exchange data.

### Networks ###
A network is a general term for a group of computers, printers, or any other device that wants to share data. Network types include LAN, HAN, CAN, MAN, WAN, BAN, or VPN.

### Topology ###
![image2](https://www.freecodecamp.org/news/content/images/size/w1000/2021/11/2-Network-Topology-Types.png)

### The OSI model consists of 7 layers of networking ###
In the OSI model, layers are organized from the most tangible and most physical, to less tangible and less physical but closer to the end user.
- Please | Physical Layer
- Do | Data Link Layer
- Not | Network Layer
- Tell (the) | Transport Layer
- Secret | Session Layer
- Password (to) | Presentation Layer
- Anyone | Application Layer

[reference](https://www.freecodecamp.org/news/osi-model-networking-layers-explained-in-plain-english/)


## What is Socket.IO ##
Socket.IO is a library that enables low-latency, bidirectional and event-based communication between a client and a server.It is built on top of the WebSocket protocol and provides additional guarantees like fallback to HTTP long-polling or automatic reconnection.
![image3](https://socket.io/images/bidirectional-communication2.png)

### Why we use Socket.IO ###
Socket.IO allows bi-directional communication between client and server. Bi-directional communications are enabled when a client has Socket.IO in the browser, and a server has also integrated the Socket.IO package. While data can be sent in a number of forms, JSON is the simplest.

### Features ###
- HTTP long-polling fallback
- Automatic reconnection
- Packet buffering
- Acknowledgements
- Broadcasting
- Multiplexing

## Server API ##
![image4](https://socket.io/images/server-class-diagram-server.png)

### *[Source01](https://socket.io/docs/v4/)*  *[Source02](https://socket.io/docs/v4/server-api)*
