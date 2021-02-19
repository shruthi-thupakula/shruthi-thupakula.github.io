## OSI Model

- The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system.
- The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.
- The OSI model has 7 Layers:

1.  **Physical Layer:** An application that communicates with other computers that corresponds to the application's communication service.
    - It is responsible for sending bits from one computer to another. It deals with the physical connectivity of two different stations. And it provides its services to Data-link layer.
1.  **Data Link Layer:** It defines how to transfer data on a single link.
    - It takes the data bits and “frames,” and creates packets of the data. It transmits bits via the physical layers.
1.  **Network Layer:** This layer defines the end-to-end packet transport, which defines the logical addresses.
    - It delivers packets from source to destination across multiple links (networks). It also divides the outgoing messages into packets and to assemble incoming packets into messages for higher levels.
1.  **Transport Layer:** It has a responsible for delivering data to the appropriate application process on the host computers.
1.  **Session Layer:** It controls the connections between computers.
1.  **Presentation Layer:** The main function of this layer is to define the data format and encryption. And it prepares data for the application layer.
1.  **Application Layer:** An application that communicates with other computers that corresponds to the application's communication service. It is used by end-user software such as web browsers and email clients.

## Deadlock

- In general deadlock is a problem where two or more processes are blocked.
- It is a situation when 2 processes sharing the same resource are effectively preventing each other from accessing the resources.
- Conditions for Deadlock- Mutual Exclusion, Hold and Wait, No preemption, Circular wait.

## Router & Switch

**Router:** A router is a networking device that connects a local network to other local networks. It is used to identify the shortest path between source and destination by connecting different networks.It works on network layer.

**Switch:** A switch is a device that is used to connect many devices together on a computer network. It works on data link layer.

**Differences between Router & Switch:**

- Router and Switch are both network connecting devices.
- A router interconnects various switches with their respective networks. As against, a switch is used to interconnect various devices to form a network.
- For data transmission Router uses IP address and Switch uses MAC address.
- Router used for connecting two or more networks. Switch used for connecting two or more nodes in the same network (L2) or different network (L3).

## Subnetting

- Subnetting is a process of dividing a large IP network into smaller IP networks.
- Subnet mask is used to divide an IP address into two parts. One part identifies the host (computer), the other part identifies the network to which it belongs.
- It increases routing efficiency, enhances the security of the network and reduces the size of the broadcast domain.

## DHCP

- Dynamic Host Configuration Protocol.
- DHCP is a network management protocol that automatically assigns IP addresses and default gateways to client devices.

**DORA Process in DHCP:**

- DORA is a sequence of messages of the DHCP process. The DHCP Server and DHCP Client exchanges some message and after that DHCP provide an IP address to DHCP client. It has four messages.

1. **Discover:** The DHCP client wants to discover a DHCP Server and sends a DHCP Discover message.
1. **Offer:** As soon as DHCP Server receives Client Discover message, the DHCP server reply to DHCP client as an offer message.
1. **Request:** The DHCP client machine receives the DHCP Offer message and replies with a DHCP request message. This message basically tells the DHCP server that I’m fine with this IP address. Please allocate this IP address to me.
1. **Acknowledgment:** DHCP acknowledge message is the last message of the DORA process. It is sent by the DHCP Server to DHCP Client. This message is a reply to the DHCP Request message.

**DHCP (DORA Process "Broadcast vs Unicast" ):**

- In DORA process, the discover and request message is broadcast, the offer and the acknowledgement message is broadcast or unicast depending upon the value of broadcast flag. If the value of broadcast flag is 1,then the offer and acknowledgement message is broadcast and if 0,the messages are unicast.

**DHCP Address Allocation Methods:**

1. Automatic allocation. —The DHCP server assigns a permanent IP address to a client from its. IP Pools. ...
2. Dynamic allocation. —The DHCP server assigns a reusable IP address from. IP Pools. ...
3. Static allocation. —The network administrator chooses the IP address to assign to the client and the DHCP server sends it to the client.

## APIPA

- Automatic Private IP Addressing (APIPA) is a feature of Windows-based operating systems that enables a computer to automatically assign itself an IP address when there is no Dynamic Host Configuration Protocol (DHCP) server available to perform that function.

## Broadcast Domain

- A broadcast domain is a collection of devices that receive broadcast traffic from each other.
- In which all nodes can reach each other by broadcast at the data link layer. A broadcast domain can be within the same LAN segment
- Switches will forward broadcast traffic to all interfaces (except the one where it originated from).

## DNS

- DNS stands for Domain Name System. The main function of DNS is to translate domain names into IP Addresses, which computers can understand.
- It also provides a list of mail servers which accept Emails for each domain name.

- 3 types of DNS queries—recursive, iterative, and non-recursive
- 3 types of DNS servers—DNS Resolver, DNS Root Server and Authoritative Name Server

**DNS Query Process:**

- DNS Query is a request sent from a DNS Client to a DNS Server, asking for the IP Address related with a Fully Qualified Domain Name.
- When you open your browser and type in “www.amazon.com”, or a DNS client needs to look up a name used in a program, it queries DNS servers to resolve the name. Each query message the client sends contains three pieces of information, specifying a question for the DNS server to answer:

- DNS domain name — stated as a fully qualified domain name (FQDN) such as “www.amazon.com”
- query type — which can either specify a resource record by type or a specialized type of query operation such as A, CNAME, NS etc.
- class — for the DNS domain name such as IN (Internet)

## Port

- It's a specific number on which some server can run.
- Port number: A port is identified for each transport protocol and address combination by a 16-bit unsigned number, known as the port number.
- 20 - File Transfer Protocol (FTP) Data Transfer
- 21 - File Transfer Protocol (FTP) Command Control
- 22 - Secure Shell (SSH)
- 23 - Telnet - Remote login service, unencrypted text messages
- 25 - Simple Mail Transfer Protocol (SMTP) E-mail Routing
- 53 - Domain Name System (DNS) service
- 80 - Hypertext Transfer Protocol (HTTP) used in World Wide Web
- 443 - HTTPS over TLS/SSL

## Seq No & Ack No

- Sequence Number is a ordered list of numbers governed by a pattern.
- Acknowledgement number is the sequence number of the next byte the receiver expects to receive.

## SSL

- It stands for Secure Sockets Layer.
- This protocol for web browsers and servers that allows for the authentication, encryption and decryption of data sent over the Internet.
- when SSL is used to secure communication between a web browser and a web server. This turns a website's address from HTTP to HTTPS, the 'S' standing for 'secure'.
- It is used to secure credit card transactions, data transfer and logins.

**SSL Handshake:**

- The main purpose of an SSL handshake is to provide privacy and data integrity for communication between a server and a client. During the Handshake, server and client will exchange important information required to establish a secure connection.

**TLS Handshake:**

- The Transport Layer Security (TLS) Handshake Protocol is responsible for the authentication and key exchange necessary to establish secure sessions.
- TLS handshake involves a series of steps, which accomplish the three main tasks :
  - exchanging encryption capabilities,
  - authenticating the SSL certificate and
  - exchanging/generating a session key.

## TCP Handshake

**TCP 3-Way Handshake Process:** TCP uses the 3-way handshake process to establish a connection between two devices before transmitting the data. After the establishment of the connection, the data transfer takes place between the devices.

1. Synchronize: Client sends the Synchronize to the server.
1. Synchronize and Acknowledge: Server replies with the Synchronize and Acknowledge to the client.
1. Acknowledgement: Client sends the ACK to the server.

- After which the connection needs to be terminated, which is also done by using the 3-way handshake process. The secure and reliable connection is established to reserve the CPU, buffer, and bandwidth of the devices to communicate properly.
- It is a must to free these resources by terminating the connection after data transmission.
- TCP 3-way handshake process can be used to establish and terminate connections in the network in a secure way.

## Packet Tracing

- Packet tracer is a network simulator used for configuring and creating the virtual cisco devices and network.
- It allows users to create network topologies.
- Most importantly, Packet Tracer helps students and instructors create their own virtual “network worlds” for experimentation and explanation of networking concepts and technologies.

## TCP & UDP

Differences:

- TCP is a connection-oriented protocol, whereas UDP is a connectionless protocol.
- The speed for TCP is slower while the speed of UDP is faster.
- TCP uses handshake protocol like SYN, SYN-ACK, ACK while UDP uses no handshake protocols.
- TCP does error checking and also makes error recovery, on the other hand, UDP performs error checking, but it discards erroneous packets.
- TCP has acknowledgment segments, but UDP does not have any acknowledgment segment.
- TCP is heavy-weight, and UDP is lightweight.
- TCP is reliable as it guarantees delivery of data to the destination router.The delivery of data to the destination cannot be guaranteed in UDP.

## Flow & Error control

- Flow control is meant only for the transmission of data from sender to receiver. It prevents the loss of data and avoid over running of receive buffers.
- Error control is meant for the transmission of error free data from sender to receiver. It is used to detect and correct the error occurred in the code.
- Flow & Error Control techniques are : Stop&Wait Protocol and Sliding Window Protocol.

## Firewall

- Firewall is a network security device that monitors incoming and outgoing network traffic and blocks data pockets based on a set of security rules.
- It protects from internet malware's and viruses.It helps to protect more from the attacking viruses from internet.
- There are software and hardware firewalls: A hardware firewall is physical, like a broadband router — stored between our network and gateway. And software firewall is internal — a program on our computer that works through port numbers and applications.
- There also cloud-based firewalls(Firewall as a Service (FaaS)). Its similar to hardware firewalls,with security.

Types:

1. Hardware Firewall
1. Software Firewall
1. Stateful Inspection Firewalls
1. Packet Filtering Firewall
1. Application firewall
1. Next-generation Firewall (NGFW)
1. Telephony Related Firewalls

Advantages:

- Better Privacy
- Prevent Hackers
- Access Control

Disadvantages:

- Cost
- User Restriction
- Performance
- Malware Attacks
- Complex Operations
