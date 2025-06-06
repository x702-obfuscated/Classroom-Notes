TODO:

A socket consists of both a host's IP address and a process's TCP or UDP port with a colon seperating the values.

```
IP_Address : Port_Number
|--------Socket--------|
```

|IP Address:Port| 255.255.255.255:65535|
|:-:|:-:|


A `session` is a temporary, interactive exchange of information between two or more devices, applications, or users over a network.

<br>



# `Ports-Protocols-Services`

---

Covered in this file:
1. [`Protocols`](#protocols)
1. [`Ports`](#ports)
1. [`Services`](#services)
1. [`Common Ports Protocols and Services`](#common-ports-protocols-and-services)


<br>

___

<br>

# `Protocols`

A `protocol` is a set of rules and conventions that define how data is transmitted and processed over a network or communication system. 
> * `Protocols` establish the procedures for data exchange, ensuring that devices and systems can communicate effectively and understand each other. 

<br>

[Back To Top](#ports-protocols-services)
___

<br>

# `Ports`
*Ports are defined by the Transmission Control Protocol (TCP) and the User Datagram Protocol (UDP) at the 4th layer of the OSI model and the TCP/IP model.* 

A `Port` serves as a communication endpoint for applications and services on a device. It helps in directing data to the correct application or service by providing a unique number associated with that service.
* Ports are numbers assigned to processes such as applications or services running on a computing device. 
* Port numbers are used to find a process running on a computer. 

<br>

A `Port Number` is a 16-bit integer ranging from 0 to 65535, and is used to uniquely identify a service or application on a device.

<br>

`Well-Known Ports`: Range from port 0 to port 1023 and are used by widely recognized services and protocols(ex. port 80 for HTTP, port 443 for HTTPS)

<br>

`Registered Ports`: range from port 1024 to port 49151, and are used by software applications that are not universally recognized but still need consistent port assignments.

<br>

`Dynamic/Ephemeral Ports`: ranges from port 49152 to port 65535, and are used temporarily by client applications for outgoing connections. These ports are assigned dynamically by the operating system.

<br>

`Private Ports` are ports assigned by a network admin that is difference from a well-known port number for a service. 

<br> 


## `Transport Layer Incoming and Outgoing Connections:`
* Client applications use `ephemeral ports` for outgoing connections to servers. 
>   * These ports are assigned by the operating system and are used for the duration of the connection.

<br>

* Servers use specific port number assignments to list for incoming connection from clients. 
>   * For example, a web server listens on port 80 for HTTP requests. 

`TCP Ports:`
> TCP ports are used for connection oriented communication such as loading a webpage. 

`UDP Ports:`
> UDP ports are used for connectionless communications such as streaming video. 


<br>

[Back To Top](#ports-protocols-services)
___

<br>

# `Services`

`Networking services` refer to a range of functionalities and operations provided over a network that facilitate communication, resource sharing, and data management between devices and systems. 
> * These services are essential for the effective operation and management of networked environments, enabling various applications and interactions. 

### Network Service Examples:
> * File Transfer Protocol (FTP)  
> * Secure File Transfer Protocol (SFTP)  
> * Simple Mail Transfer Protocol (SMTP)
> * Internet Message Access Protocol (IMAP)
> * Post Office Protocol version 3 (POP3)
> * Hypertext Transfer Protocol (HTTP)
> * Hypertext Transfer Protocol Secure (HTTPS)
> * Domain Name System (DNS)
> * Dynamic Host Configuration Protocol (DHCP)
> * Network Time Protocol (NTP)
> * Remote Desktop Protocol (RDP)




<br>

[Back To Top](#ports-protocols-services)
___

<br>

# `Common Ports Protocols and Services`

*This is not a comprehensive list; it is intend to show the most commonly encountered ports and protocols.*

| TCP/IP Layer | Transport Protocol | Service | Port | Purpose |
|:------------:|:------------------:|:-------|:----:|:--------|
| 5 | TCP/UDP | File Transfer Protocol (FTP-data) | 20 | Transfer files between FTP client and FTP server |
| 5 | TCP | File Transfer Protocol (FTP-Control) | 21 | Manages the connection between FTP client and FTP server |
| 5 | TCP | Secure Shell (SSH)<br>Secure Copy Protocol (SCP)<br>Secure FTP (SFTP) | 22 | Provides a secure remote shell service for accessing and managing a remote connection<br>Also allows for encrypted file transfer |
| 5 | TCP | Teletype Network (TelNet) | 23 | Provides a text-based terminal connection to a remote computer |
| 5 | TCP | Simple Mail Transfer Protocol (SMTP) | 25 | Sends email from one server to another |
| 5 | UDP | Domain Name System (DNS) | 53 | Translates domain names into IP addresses |
| 5 | UDP | Trivial File Transfer Protocol (TFTP) | 69 | Simple, lightweight file transfer protocol often used for booting devices or transferring configs |
| 5 | TCP | Hypertext Transfer Protocol (HTTP) | 80 | Transfers web pages from web server to web browser |
| 5 | TCP | Post Office Protocol (POP3) | 110 | Retrieves email messages from an email server to a POP3 client |
| 5 | UDP | Network Time Protocol (NTP) | 123 | Synchronizes clocks across devices on a network |
| 5 | TCP | Internet Message Access Protocol (IMAP4) | 143 | Retrieves and manages email messages on an email server |
| 5 | UDP | Simple Network Management Protocol (SNMP) | 161 | Monitors and manages devices on IP networks (like routers, switches, servers) |
| 5 | UDP | SNMP Trap | 162 | Used by SNMP agents to send alerts or traps to the management system |
| 5 | TCP | Hypertext Transfer Protocol Secure (HTTPS) | 443 | TLS/SSL version of HTTP |
| 5 | TCP | Server Message Block (SMB) | 445 | Common Windows network protocol for sharing files and resources |
| 5 | TCP | Lightweight Directory Access Protocol (LDAP) | 389 | Accesses and maintains distributed directory information services over a network |
| 5 | TCP | LDAP Secure (LDAPS) | 636 | Secure version of LDAP using SSL/TLS for encryption |
| 5 | TCP | Simple Mail Transfer Protocol Secure (SMTPS) | 465 | TLS/SSL version of SMTP |
| 5 | TCP | File Transfer Protocol Secure (FTPS-data) | 989 | TLS/SSL version of FTP-data |
| 5 | TCP | File Transfer Protocol Secure (FTPS-control) | 990 | TLS/SSL version of FTP-control |
| 5 | TCP | Internet Message Access Protocol Secure (IMAPS) | 993 | TLS/SSL version of IMAP |
| 5 | TCP | Post Office Protocol Secure (POP3S) | 995 | TLS/SSL version of POP3 |
| 5 | UDP | Dynamic Host Configuration Protocol (DHCP) | 67,68 | Assigns IP addresses and other network configurations to devices |
| 5 | TCP | Real Time Streaming Protocol (RTSP) | 1755 | Streams multimedia content, audio, and video over a network |
| 5 | TCP | H.323 | 1720 | Protocol suite for voice, video, and data conferencing over packet-switched networks |
| 5 | TCP | Border Gateway Protocol (BGP) | 179 | Routing protocol used for exchanging routing information between autonomous systems |
| 5 | TCP | Remote Desktop Protocol (RDP) | 3389 | Provides a GUI remote desktop connection |
| 5 | TCP/UDP | Session Initiation Protocol (SIP) | 5060, 5061 | Protocol for initiating, maintaining, and terminating multimedia sessions |

<br>
<br>

| TCP/IP Layer | Protocol | Purpose |
|:------------:|:------------------:|:--------|
| 4 | Transport Control Protocol (TCP) | Connection-oriented transport protocol |
| 4 | User Datagram Protocol (UDP) | Connectionless transport protocol |
| 3 | Internet Protocol (IPv4) | Responsible for routing data across networks |
| 3 | Internet Protocol (IPv6)  | Responsible for routing data across networks |
| 3 | Internet Control Message Protocol (ICMP) | Used for exchanging control information across network devices |
| 2 | Address Resolution Protocol (ARP) | Used to map IP addresses to MAC addresses |








<br>

[Back To Top](#ports-protocols-services)
___

<br>

*Created and maintained by Mr. Merritt*