The **TCP/IP model** is a framework used to visualize how data is organized and transmitted across a network.
![[Pasted image 20240926194306.png]]
## Network access layer
- The network access layer, sometimes called the data link layer, deals with the **creation of data packets and their transmission across a network**.
- This layer corresponds to the physical hardware involved in network transmission.
- The address resolution protocol (ARP) is part of the network access layer. ARP is needed to map IP addresses to MAC addresses for local network communication.

## Internet layer
- The internet layer, sometimes referred to as the network layer, is **responsible for ensuring the delivery to the destination host**, which potentially resides on a different network.
- ensures IP addresses are attached to data packets
- determines which protocol is responsible for delivering the data packets and ensures the delivery to the destination host, example: **Internet Protocol (IP)**, **Internet Control Message Protocol (ICMP)**

## Transport layer
- responsible for delivering data between two systems or networks and includes protocols to control the flow of traffic across a network
- TCP and UDP are the two transport protocols that occur at this layer.
	- **Transmission Control Protocol** - protocol that allows two devices to form a connection and stream data
	- **User Datagram Protocol** - connectionless protocol that does not establish a connection between devices before transmissions. it doesn't require a handshake, (no 3 way handshake)

## Application layer
- The application layer in the TCP/IP model is similar to the application, presentation, and session layers of the OSI model.
- responsible for making network requests or responding to requests
- Protocols in the application layer determine how the data packets will interact with receiving devices
- Some common protocols used on this layer are: 
	- Hypertext transfer protocol (HTTP)
	- Simple mail transfer protocol (SMTP)
	- Secure shell (SSH)
	- File transfer protocol (FTP)
	- Domain name system (DNS)

![[Pasted image 20240926195043.png]]