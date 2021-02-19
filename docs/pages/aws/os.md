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

## Boot Process

The Boot process of a computer is when we power the motherboard "ON" and it turns on the BIOS (chip), which controls our input-output with the computer completely. The BIOS then select a drive to Boot to (drive C: most likely) and the system powers on. Windows or the operating system then takes over and controls all the components: CPU, GPU, drives, drivers, etc.

- Basically “Boot Process” A CPU gets its instructions from memory. The CPU reads instruction from the BIOS and searches for the hard disks, CD drives and other hardware. The BIOS program looks at the first sector for boot code.
- Linux have 6 stages of Boot:

1. BIOS ( Basic Input/Output System )
1. MBR ( Master boot Record )
1. GRUB ( Grand Unified Boot Loader )
1. Kernel
1. init
1. run level ( init 0 — init 6 )

## Memory Management

In operating systems, memory management is the function responsible for managing the computer's primary memory.

- The memory management function keeps track of the status of each memory location, either allocated or free.
- It determines how memory is allocated among competing processes and how much they are allowed.
- When memory is allocated it determines which memory locations will be assigned.
- It tracks when memory is unallocated and updates the status.

**Paging:**

- Paging is a method of writing and reading data from a secondary storage(Drive) for use in primary storage(RAM). - When a computer runs out of RAM, the operating system (OS) will move pages of memory over to the computer’s hard disk to free up RAM for other processes.
- This ensures that the operating system will never run out of memory and crash. Too much reliance on memory paging can impair performance, however, because random access memory operates much faster than disk memory.
- This means the operating system has to wait for the disk to catch up every time a page is swapped; the more a work.

**Segmentation:**

- Segmentation is a virtual process that creates address spaces of various sizes in a computer system, called segments. Each segment is a different virtual address space that directly corresponds to process objects.This process speed retrieval.

**Framing:**

- Framing is the smallest unit of data for memory management in a virtual memory operating system. A frame refers to a storage frame. In terms of physical memory it is a fixed sized block in physical memory space

**Virtual Memory:**
Virtual memory is an area of a computer system’s secondary memory storage space (such as a hard disk or solid state drive) which acts as if it were a part of the system’s primary memory(RAM).

- Virtual memory is a portion of an HDD or SSD that is reserved to emulate RAM.

## Buffer & Caching

- Buffer: Buffer temporarily stores data that is being transmitted from one place to another. The act of storing data temporarily in the buffer is called buffering.Buffering helps in matching the speed between the sender and receiver of the data stream. If the sender’s transmission speed is slower than receiver, then a buffer is created in main memory of the receiver, and it accumulates the bytes received from the sender.

- Caching : Cache is a memory implemented in the processor that stores the copy of original data. The idea behind caching is that the recently accessed disk blocks must be stored in the cache memory so that when the user again needs to access the same disk blocks, it can be handled locally through cache memory avoiding the network traffic.
- Buffering vs Caching:
  - Buffer always carry the original data to be sent to the receiver. However, cache carries the copy of original data.

## NTP

- Network Time Protocol is used to synchronize computer clock times in a network.
- NTP is an Internet standard protocol.
- NTP applies to both the protocol and the client-server programs that run on computers.
- NTP provides an accurate timing mechanism using Coordinated Universal Time (UTC).

**Managing Users and groups:**

These operations are performed using the following commands:

- adduser : add a user to the system.
- userdel : delete a user account and related files.
- addgroup : add a group to the system.
- delgroup : remove a group from the system.
- usermod : modify a user account.
- chage : change user password expiry information.
- sudo: run one or more commands as another user
