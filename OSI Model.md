![[Pasted image 20240926195244.png]]

## The TCP/IP model vs. the OSI model
- The **TCP/IP model** is a framework used to visualize how data is organized and transmitted across a network.
- The **OSI model** is a standardized concept that describes the seven layers computers use to communicate and send data over the network. Network and security professionals often use this model to communicate with each other about potential sources of problems or security threats when they occur.
- Defines how information from one device should transmit to other device
---
## Layer 1: Physical layer
- the physical layer corresponds to the physical hardware involved in network transmission.
- Hubs, modems, and the cables and wiring that connect them are all considered part of the physical layer

## Layer 2: Data link layer
- The data link layer organizes sending and receiving data packets within a single network
- Can route data using mac addresses
- The data link layer is home to switches on the local network and network interface cards on local devices
- Protocols like network control protocol (NCP), high-level data link control (HDLC), and synchronous data link control protocol (SDLC) are used at the data link layer.

## Layer 3: Network layer
- The network layer oversees receiving the frames from the data link layer (layer 2) and delivers them to the intended destination.
- can route data using ip addresses but can also work at layer 2
- Data packets allow communication between two networks. These packets include IP addresses that tell routers where to send them.
- They are routed from the sending network to the receiving network.

## Layer 4: Transport layer
- The transport layer is responsible for delivering data between devices.
- Basically this is for Ports
- This layer also handles the speed of data transfer, flow of the transfer, and breaking data down into smaller segments to make them easier to transport.
- These segments need to be reassembled at their destination so they can be processed at the session layer (layer 5)
- TCP and UDP are transport layer protocols.

## Layer 5: Session layer
- A session describes when a connection is established between two devices. An open session allows the devices to communicate with each other (came from mainframe and dumb terminals concept)
- distinguishes a session between 2 users 
- http cookies are used here 
- Sessions include a request and response between applications.
- Functions in the session layer are, **requests for service from processes** in the presentation layer (layer 6) and **send requests for services** to the transport layer (layer 4).

## Layer 6: Presentation layer
- Functions at the presentation layer involve data translation and encryption for the network
- Tells us how to arrange the data that has arrived(bits)
- http ascii encoding is 8 bit encoding method 
- other encoding methods can be used as well like JPEG, MPEG, and SSL/TLS
- Some formatting functions that occur at layer 6 include encryption, compression, and confirmation that the character code set can be interpreted on the receiving system
- One example of encryption that takes place at this layer is SSL, which encrypts data between web servers and browsers as part of websites with HTTPS.

## Layer 7: Application layer
- The application layer includes processes that directly involve the everyday user. This layer includes all of the networking protocols that software applications use to connect a user to the internet.
- Basically tells what to do with this decoded info now
- GET(Fetches the page), POST(submits the data), PUT(updates the data), DELETE(deletes), TRACE(echoes received request to client)
- An example of a type of communication that happens at the application layer is using a web browser. The internet browser uses HTTP or HTTPS to send and receive information from the website server.