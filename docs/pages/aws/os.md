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

## Network Protocols

- It has set of rules that determines how data is transmitted between different devices in the same network.
  Types of Network Protocols:

1.  **File Transfer Protocol (FTP):** It allows users to transfer files from one machine to another. Types of files may include program files, multimedia files, text files, and documents, etc.
1.  **Hyper Text Transfer Protocol (HTTP):** It is used for transferring data between the client browser (request) and the web server (response) in the hypertext format.
1.  **Hyper Text Transfer Protocol Secure (HTTPS):** It is a standard protocol to secure the communication among two computers one using the browser and other fetching data from web server.
1.  **Simple mail transport Protocol (SMTP):** It is designed to send and distribute outgoing E-Mail.
1.  **Transmission Control Protocol (TCP):** It is a communications standard that enables application programs and computing devices to exchange messages over a network.

    - It is designed to send packets across the internet and ensure the successful delivery of data and messages over networks.
    - TCP is used extensively by many internet applications, including the World Wide Web (WWW), email, File Transfer Protocol, Secure Shell, peer-to-peer file sharing, and streaming media.

1.  **Internet Protocol (IP):** It is designed explicitly as addressing protocol. It is mostly used with TCP. The IP addresses in packets help in routing them through different nodes in a network until it reaches the destination system. TCP/IP is the most popular protocol connecting the networks.
1.  **User Datagram Protocol (UDP):** It is a Transport Layer protocol. UDP is a part of Internet Protocol.Unlike TCP, it is unreliable and connectionless protocol. So, there is no need to establish connection prior to data transfer.
1.  **Post office Protocol (POP):** POP3 is designed for receiving incoming E-mails.
1.  **Telnet:** Telnet is a set of rules designed for connecting one system with another. The connecting process here is termed as remote login. The system which requests for connection is the local computer, and the system which accepts the connection is the remote computer.
1.  **Gopher:** Gopher is a collection of rules implemented for searching, retrieving as well as displaying documents from isolated sites. Gopher also works on the client/server principle.

## Deadlock

- In general deadlock is a problem where two or more processes are blocked.
- It is a situation when 2 processes sharing the same resource are effectively preventing each other from accessing the resources.
- Conditions for Deadlock- Mutual Exclusion, Hold and Wait, No preemption, Circular wait.

## SSL

- It stands for Secure Sockets Layer.
- This protocol for web browsers and servers that allows for the authentication, encryption and decryption of data sent over the Internet.
- when SSL is used to secure communication between a web browser and a web server. This turns a website's address from HTTP to HTTPS, the 'S' standing for 'secure'.
- It is used to secure credit card transactions, data transfer and logins.

**SSL Handshake**

- The main purpose of an SSL handshake is to provide privacy and data integrity for communication between a server and a client. During the Handshake, server and client will exchange important information required to establish a secure connection.

## TCP Handshake

**TCP 3-Way Handshake Process:** TCP uses the 3-way handshake process to establish a connection between two devices before transmitting the data. After the establishment of the connection, the data transfer takes place between the devices.

1. Synchronize: Client sends the Synchronize to the server.
1. Synchronize and Acknowledge: Server replies with the Synchronize and Acknowledge to the client.
1. Acknowledgement: Client sends the ACK to the server.

- After which the connection needs to be terminated, which is also done by using the 3-way handshake process. The secure and reliable connection is established to reserve the CPU, buffer, and bandwidth of the devices to communicate properly.
- It is a must to free these resources by terminating the connection after data transmission.
- TCP 3-way handshake process can be used to establish and terminate connections in the network in a secure way.
