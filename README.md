# CCNA

**Open systems Interconnection (OSI) Model**

The OSI Model is a conceptual framework used to understand how data travels across a network. It divides network communication into seven layers, with each responsible for a specific function.

By breaking networking into layers, devices and protocols can communicate using a common structure, making networks
easier to design, troubleshoot, and understand.

When data is sent from one device to another, it travels down the OSI layers on the sender's device, across the network, and then up the OSI layers on the receiver's device.

**The Seven Layers**

Application [7] Data

Presentation [6] Data

Session [5] Data

Transport [4] Segment

Network [3] Packet

Data-Link [2] Frame

Physical [1] Bits

A common way to remember the layers from bottom to top is:

*Please Do Not Throw Sausage Pizza Away*

(Physical, Data-Link, Network, Transport, Session, Presentation, Application).

# OSI Model Overview

**Layer 1: Physical Layer**

The Physical Layer is responsible for the transmission of raw bits across a physical medium. It includes the hardware used to send and receive data, such as cables, wires, connectors, network interface ports, hubs, and electrical or wireless signals. This layer focuses on how data physically travels from one device to another.

**Layer 2: Data Link Layer**

The Data Link Layer is responsible for transferring data between devices on the same local network. Switching takes place at this layer using MAC (Media Access Control) addresses. Every network device has a Network Interface Card (NIC) with a unique MAC address that identifies it on the network.

At Layer 2, data is encapsulated into a frame. A frame contains a header and a trailer. The trailer includes a Frame Check Sequence (FCS), which is used to detect errors during transmission and ensure data integrity.

Characteristics:

- Uses MAC addresses for communication.
- Switches operate at this layer.
- Data unit: Frame.
- Includes a Frame Check Sequence (FCS) for error checking.
- Typically consists of one broadcast domain and one collision domain per switched port.

**Layer 3: Network Layer**

The Network Layer is responsible for routing data between different networks. It uses IP (Internet Protocol) addresses to identify the source and destination of data. Routers operate at this layer and determine the best path for data to travel across interconnected networks.

At Layer 3, data is encapsulated into a packet, which contains addressing information needed for routing.

Characteristics:

- Uses IP addresses.
- Routers operate at this layer.
- Data unit: Packet.
- Responsible for path selection and routing.
- A router separates broadcast domains, creating multiple collision domains and separate broadcast domains.

**Layer 4: Transport Layer**

The Transport Layer ensures data is delivered correctly between devices and applications. The two main protocols used at this layer are TCP and UDP.

TCP (Transmission Control Protocol)

TCP provides reliable communication by establishing a connection before data is transmitted. It uses a three-way handshake and performs error checking, sequencing, and retransmission of lost data.

Advantages:

- Highly reliable.
- Error recovery and acknowledgment.
- Guarantees data arrives in the correct order.

Disadvantage:

- Slower due to additional checks and overhead.
- UDP (User Datagram Protocol)

UDP is a connectionless protocol that sends data without establishing a connection first. It does not guarantee delivery, sequencing, or error recovery, making it faster than TCP.

Advantages:

- Faster transmission.
- Lower overhead.

Disadvantage:

- Less reliable because packets may be lost or arrive out of order.

**Layer 5: Session Layer**

The Session Layer is responsible for establishing, managing, and terminating communication sessions between applications. It keeps communication organised and ensures that sessions remain active for the duration of data exchange.

Examples include:

- Logging into a remote system.
- Maintaining a video conference session.
- Managing communication between client and server applications.

**Layer 6: Presentation Layer**

The Presentation Layer is responsible for how data is presented to the application layer. It translates, formats, encrypts, and compresses data so that different systems can understand and use it correctly.

Functions include:

- Data formatting and translation.
- Encryption and decryption.
- Data compression and decompression.

**Layer 7: Application Layer**

The Application Layer is the layer closest to the end user. It provides network services that applications use to communicate over a network.

Examples of applications and protocols:

- Web browsers (HTTP/HTTPS)
- Email services (SMTP, POP3, IMAP)
- File transfer (FTP)
- Domain name services (DNS)

This layer allows users to access network resources and services through everyday applications.
