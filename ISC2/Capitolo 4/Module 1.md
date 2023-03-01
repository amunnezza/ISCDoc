# Module 1: Understand Computer Networking

Domain D4.1.1, D4.1.2

## Module Objectives

-   L4.1.1 Recognize common networking terms and models.
-   L4.1.2 Identify common protocols and ports and their secure counterparts when presented with a network diagram.

## Video UnderstandCompNetwork.mkv


Transcript
_Manny_: One of the biggest issues in cybersecurity is that computers are all linked together, sometimes by physical networks within a building, and almost always via the Internet, so it's easy for viruses and other threats to move rapidly through networks. 
_Tasha_: That's right, and cyber threats and attacks are getting more sophisticated all the time. This aspect of cybersecurity is always evolving. Let's find out more.

# What is Networking

A network is simply two or more computers linked together to share data, information or resources.

To properly establish secure data communications, it is important to explore all of the technologies involved in computer communications. From [hardware](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_04/module_01/ch04_m01-What_is_Networking.html?d2lSessionVal=Mi4hLS4lYYLy6kUwwSCV3JUf6&ou=9541&d2l_body_type=3#) and [software](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_04/module_01/ch04_m01-What_is_Networking.html?d2lSessionVal=Mi4hLS4lYYLy6kUwwSCV3JUf6&ou=9541&d2l_body_type=3#) to 
>[!protocols]- 
> A set of rules (formats and procedures) to implement and control some type of association (that is communication) between systems. NIST SP 800-82 REV.2

and 
> [!encryption]- 
> The process and act of conveting the message from its plaintext to ciphertext. Sometimes it is also referred to ad enciphering. The two terms are cometimes used interchangeably in iterature and have similar meaning. 

 and beyond, there are many details, standards and procedures to be familiar with.
## Types of Networks

There are two basic types of networks:

-   **Local area network (LAN)** - A local area network (LAN) is a network typically spanning a single floor or building. This is commonly a limited geographical area.
-   **Wide area network (WAN**) - Wide area network (WAN) is the term usually assigned to the long-distance connections between geographically remote networks.

## Network Devices

_ick on each tab below to learn more._ 

[Hub]
Hubs are used to connect multiple devices in a network. They’re less likely to be seen in business or corporate networks than in home networks. Hubs are wired devices and are not as smart as switches or routers.
"image of a switch"

[Switch]
Rather than using a hub, you might consider using a switch, or what is also known as an intelligent hub. Switches are wired devices that know the addresses of the devices connected to them and route traffic to that port/device rather than retransmitting to all devices.

Offering greater efficiency for traffic delivery and improving the overall throughput of data, switches are smarter than hubs, but not as smart as routers. Switches can also create separate 
>[!broadcast]-
>Broadcast transmission is a one-to-many (one to everyone) form of sending internet traffic 

domains when used to create 
>[!VLANs]- 
>A virtual local area network is a logical group of devices that appear to be on the same LAN despite their geographical distribution. 

 which will be discussed later.

[Router]
Routers are used to control traffic flow on networks and are often used to connect similar networks and control traffic flow between them. Routers can be wired or wireless and can connect multiple switches. Smarter than hubs and switches, routers determine the most efficient “route” for the traffic to flow across the network.

[Firewall]
Firewalls are essential tools in managing and controlling network traffic and protecting the network. A firewall is a network device used to filter traffic. It is typically deployed between a private network and the internet, but it can also be deployed between departments (segmented networks) within an organization (overall network). Firewalls filter traffic based on a defined set of rules, also called filters or access control lists.

[Server]
A server is a computer that provides information to other computers on a network. Some common servers are web servers, email servers, print servers, database servers and file servers. All of these are, by design, networked and accessed in some way by a client computer. Servers are usually secured differently than workstations to protect the information they contain.

[Endpoint]
Endpoints are the ends of a network communication link. One end is often at a server where a resource resides, and the other end is often a client making a request to use a network resource. An endpoint can be another server, desktop workstation, laptop, tablet, mobile phone or any other end user device.


## Other Networking Terms

### Ethernet![image of an ethernet cable](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_04/assets/EDU-ELCC-70260h-ethernet-icon-v01.svg?_&d2lSessionVal=yBjfRYCKPbzWFncFn40KvvFLX&ou=9541 "image of an ethernet cable")

Ethernet (IEEE 802.3) is a standard that defines wired connections of networked devices. This standard defines the way data is formatted over the wire to ensure disparate devices can communicate over the same cables.

### Device Address

-   ![image of MAC address on a device](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_04/assets/EDU-ELCC-70260e-mac_address-icon-v01.svg?_&d2lSessionVal=yBjfRYCKPbzWFncFn40KvvFLX&ou=9541 "image of MAC address on a device")**Media Access Control (MAC) Address** - Every network device is assigned a Media Access Control (MAC) address. An example is 00-13-02-1F-58-F5. The first 3 [bytes](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_04/module_01/ch04_m01-What_is_Networking.html?d2lSessionVal=yBjfRYCKPbzWFncFn40KvvFLX&ou=9541&d2l_body_type=3#) (24 bits) of the address denote the vendor or manufacturer of the physical network interface. No two devices can have the same MAC address in the same local network; otherwise an address conflict occurs.
-   ![image representing the IP address of a laptop](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_04/assets/EDU-ELCC-70260i-ip_address-icon-v01.svg?_&d2lSessionVal=yBjfRYCKPbzWFncFn40KvvFLX&ou=9541 "image representing the IP address of a laptop")**Internet Protocol (IP) Address** - While MAC addresses are generally assigned in the firmware of the interface, IP hosts associate that address with a unique logical address. This logical IP address represents the network interface within the network and can be useful to maintain communications when a physical device is swapped with new hardware. Examples are 192.168.1.1 and 2001:db8::ffff:0:1.

# Networking at a Glance

![[EDU-ELCC-70245a-Network_Diagram-techart-v06.svg]]

This diagram represents a small business network, which we will build upon during this lesson. The lines depict wired connections. Notice how all devices behind the firewall connect via the network switch, and the firewall lies between the network switch and the internet. 



The network diagram below represents a typical home network. Notice the primary difference between the home network and the business network is that the router, firewall, and network switch are often combined into one device supplied by your internet provider and shown here as the wireless access point.

![[EDU-ELCC-70670-techart-Networking_at_Glance-v02.svg]]

# Networking Models

Many different models, architectures and standards exist that provide ways to interconnect different hardware and software systems with each other for the purposes of sharing information, coordinating their activities and accomplishing joint or shared tasks.

Computers and networks emerge from the integration of communication devices, storage devices, processing devices, security devices, input devices, output devices, operating systems, software, services, data and people.

Translating the organization’s security needs into safe, reliable and effective network systems needs to start with a simple premise. The purpose of all communications is to exchange information and ideas between people and organizations so that they can get work done.

Those simple goals can be re-expressed in network (and security) terms such as:

-   Provide reliable, managed communications between hosts (and users)
-   Isolate functions in layers
-   Use _packets_ (Representation of data at layer 3 of the OSI model)  as the basis of communication
-   Standardize routing, addressing and control
-   Allow layers beyond internetworking to add functionality
-   Be vendor-agnostic, scalable and resilient

In the most basic form, a network model has at least two layers:

_Select each plus sign hotspot to learn more about each topic._

## Upper Layer
The upper layer, also known as the host or application layer, is responsible for managing the integrity of a connection and controlling the session as well as establishing, maintaining and terminating communication sessions between two computers. It is also responsible for transforming data received from the Application Layer into a format that any system can understand. And finally, it allows applications to communicate and determines whether a remote communication partner is available and accessible.

## Lower Layer
The lower layer is often referred to as the media or transport layer and is responsible for receiving bits from the physical connection medium and converting them into a frame. Frames are grouped into standardized sizes. Think of frames as a bucket and the bits as water. If the buckets are sized similarly and the water is contained within the buckets, the data can be transported in a controlled manner. Route data is added to the frames of data to create packets. In other words, a destination address is added to the bucket. Once we have the buckets sorted and ready to go, the host layer takes over.

# Open Systems Interconnection (OSI) Model

The OSI Model was developed to establish a common way to describe the communication structure for interconnected computer systems. The OSI model serves as an abstract framework, or theoretical model, for how protocols should function in an ideal world, on ideal hardware. Thus, the OSI model has become a common conceptual reference that is used to understand the communication of various hierarchical components from software interfaces to physical hardware.

The OSI model divides networking tasks into seven distinct layers. Each layer is responsible for performing specific tasks or operations with the goal of supporting data exchange (in other words, network communication) between two computers. The layers are interchangeably referenced by name or layer number. For example, Layer 3 is also known as the Network Layer. The layers are ordered specifically to indicate how information flows through the various levels of communication. Each layer communicates directly with the layer above and the layer below it. For example, Layer 3 communicates with both the Data Link (2) and Transport (4) layers.

The Application, Presentation, and Session Layers (5-7) are commonly referred to simply as data. However, each layer has the potential to perform encapsulation. 
>[!Encapsulation]- 
>Enforcement of data hiding and code hiding during all phases of software development and operational use. 
>Bundling ttogheter data and methods is the process of encapsulation; its opposite process may be called unpacking, revealing, or using other terms. 
>Also used to refer to taking any set of data and packaging it or hiding it in another data structure, as is common in network protocols and encryption.
>

is the addition of header and possibly a footer (trailer) data by a protocol used at that layer of the OSI model. Encapsulation is particularly important when discussing Transport, Network and Data Link layers (2-4), which all generally include some form of header. At the Physical Layer (1), the data unit is converted into binary, i.e., 01010111, and sent across physical wires such as an ethernet cable.  

It's worth mapping some common networking terminology to the OSI Model so you can see the value in the conceptual model.

Consider the following examples: 

-   When someone references an image file like a JPEG or PNG, we are talking about the Presentation Layer (6). 
-   When discussing logical ports such as NetBIOS, we are discussing the Session Layer (5).
-   When discussing TCP/UDP, we are discussing the Transport Layer (4).
-   When discussing routers sending packets, we are discussing the Network Layer (3). 
-   When discussing switches, bridges or WAPs sending frames, we are discussing the Data Link Layer (2). 

Encapsulation occurs as the data moves down the OSI model from Application to Physical. As data is encapsulated at each descending layer, the previous layer’s header, [payload]() and footer are all treated as the next layer’s payload. The data unit size increases as we move down the conceptual model and the contents continue to encapsulate.    
   
The inverse action occurs as data moves up the OSI model layers from Physical to Application. This process is known as [de-encapsulation]()  (or decapsulation). The header and footer are used to properly interpret the data payload and are then discarded. As we move up the OSI model, the data unit becomes smaller. The encapsulation/de-encapsulation process is best depicted visually below:

![[EDU-ELCC-70515-techart-osi_model-v01.jpg]]

# Transmission Control Protocol/Internet Protocol (TCP/IP)

The OSI model wasn’t the first or only attempt to streamline networking protocols or establish a common communications standard. In fact, the most widely used protocol today, 
>[!TCP/IP]- 
>Internetworking protocol model created by IETF, which specify 4 layers of functionality:
>*Link Layer* (physical communication)
>*Internet Layer* (Network to Network communication)
>*Transport Layer* (bsic channels for connections and connectionless exchange of data between hosts)
>*Application Layer* where other protocols and user applications programs make use of network services


, was developed in the early 1970s. The OSI model was not developed until the late 1970s. The TCP/IP protocol stack focuses on the core functions of networking.  
| **TCP/IP Protocol Architecture Layers** |                                                |
| --------------------------------------- | ---------------------------------------------- |
| Application Layer                       | Defines the protocols for the transport layer. |
| Transport Layer                         | Permits data to move among devices.            |
| Internet Layer                          | Creates/inserts packets.                       |
|           Network Interface Layer                              |         How data moves through the network.                                          |

The most widely used protocol suite is TCP/IP, but it is not just a single protocol; rather, it is a protocol stack comprising dozens of individual protocols. TCP/IP is a platform-independent protocol based on open standards. However, this is both a benefit and a drawback. TCP/IP can be found in just about every available operating system, but it consumes a significant amount of resources and is relatively easy to hack into because it was designed for ease of use rather than for security.

At the Application Layer, TCP/IP protocols include Telnet, [File Transfer Protocol (FTP)], [Simple Mail Transport Protocol (SMTP)], and [Domain Name Service (DNS)] (This last acronyms can be applied to three interrelated elements: a service, a physical server and a network protocol ).


The two primary Transport Layer protocols of TCP/IP are TCP and UDP. TCP is a full-duplex connection-oriented protocol, whereas UDP is a simplex connectionless protocol. In the Internet Layer, 
>[!Internet Control Message Protocol (ICMP)]-
>An IP network protocol standardized by the Internet Engineering Task Force (IETF) through RFC 792 to determine if a particular service or host is available. 

is used to determine the health of a network or a specific link. ICMP is utilized by ping, traceroute and other network management tools. The ping utility employs ICMP echo packets and bounces them off remote systems. Thus, you can use ping to determine whether the remote system is online, whether the remote system is responding promptly, whether the intermediary systems are supporting communications, and the level of performance efficiency at which the intermediary systems are communicating.
![[EDU-ELCC-70520-techart-tcpip_protocol-v04.jpg]]



 
## Knowledge Check: Networking Terms and Models
 
![[KnowTest.png]]



# Internet Protocol (IPv4 and IPv6)

IP is currently deployed and used worldwide in two major versions. IPv4 provides a 32-bit address space, which by the late 1980s was projected to be exhausted. IPv6 was introduced in December 1995 and provides a 128-bit address space along with several other important features. 

![image of IP address with first octet marked with a bracket and labeling to indicate 32 bit address, dotted decimal address, network address, and host addres]
![[EDU-ELCC-70275-techart-Internet_Protocol-v01 (1).jpg]]
IP hosts/devices associate an address with a unique logical address. An [IPv4](https://learn.isc2.org/content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_04/module_01/ch04_m01-Internet_Protocol_(IPv4_and_IPv6).html?d2lSessionVal=yBjfRYCKPbzWFncFn40KvvFLX&ou=9541&d2l_body_type=3#) address is expressed as four octets separated by a dot (.), for example, 216.12.146.140. Each octet may have a value between 0 and 255. However, 0 is the network itself (not a device on that network), and 255 is generally reserved for broadcast purposes. Each address is subdivided into two parts: the network number and the host. The network number assigned by an external organization, such as the Internet Corporation for Assigned Names and Numbers (ICANN), represents the organization’s network. The host represents the network interface within the network.  

To ease network administration, networks are typically divided into subnets. Because subnets cannot be distinguished with the addressing scheme discussed so far, a separate mechanism, the subnet mask, is used to define the part of the address used for the subnet. The mask is usually converted to decimal notation like 255.255.255.0.  

With the ever-increasing number of computers and networked devices, it is clear that IPv4 does not provide enough addresses for our needs. To overcome this shortcoming, IPv4 was sub-divided into public and private address ranges. Public addresses are limited with IPv4, but this issue was addressed in part with private addressing. Private addresses can be shared by anyone, and it is highly likely that everyone on your street is using the same address scheme.  

The nature of the addressing scheme established by IPv4 meant that network designers had to start thinking in terms of IP address reuse. IPv4 facilitated this in several ways, such as its creation of the private address groups; this allows every LAN in every SOHO (small office, home office) situation to use addresses such as 192.168.2.xxx for its internal network addresses, without fear that some other system can intercept traffic on their LAN.


This table shows the private addresses available for anyone to use:


**Range** |
-------------|
10.0.0.0 to 10.255.255.254 | 
172.16.0.0 to 172.31.255.254 |
192.168.0.0 to 192.168.255.254 |

The first octet of 127 is reserved for a computer’s loopback address. Usually, the address 127.0.0.1 is used. The loopback address is used to provide a mechanism for self-diagnosis and troubleshooting at the machine level. This mechanism allows a network administrator to treat a local machine as if it were a remote machine and ping the network interface to establish whether it is operational.

IPv6 is a modernization of IPv4, which addressed a number of weaknesses in the IPv4 environment:

-   A much larger address field: IPv6 addresses are 128 bits, which supports 2128 or 340,282,366,920,938,463,463,374,607,431,768,211,456 hosts. This ensures that we will not run out of addresses.

-   Improved security: IPsec is an optional part of IPv4 networks, but a mandatory component of IPv6 networks. This will help ensure the integrity and confidentiality of IP packets and allow communicating partners to authenticate with each other.

-   Improved quality of service (QoS): This will help services obtain an appropriate share of a network’s bandwidth.

An IPv6 address is shown as 8 groups of four digits. Instead of numeric (0-9) digits like IPv4, IPv6 addresses use the hexadecimal range (0000-ffff) and are separated by colons (:) rather than periods (.). An example IPv6 address is 2001:0db8:0000:0000:0000:ffff:0000:0001. To make it easier for humans to read and type, it can be shortened by removing the leading zeros at the beginning of each field and substituting two colons (::) for the longest consecutive zero fields. All fields must retain at least one digit. After shortening, the example address above is rendered as 2001:db8::ffff:0:1, which is much easier to type. As in IPv4, there are some addresses and ranges that are reserved for special uses:

-   ::1 is the local loopback address, used the same as 127.0.0.1 in IPv4.
-   The range 2001:db8:: to 2001:db8:ffff:ffff:ffff:ffff:ffff:ffff is reserved for documentation use, just like in the examples above.
-   fc00:: to fdff:ffff:ffff:ffff:ffff:ffff:ffff:ffff are addresses reserved for internal network use and are not routable on the internet.
 

# Knowledge check Formatting IPv6

Which of the following examples is a correctly shortened version of the address 2001:0db8:0000:0000:0000:ffff:0000:0001?

A. 2001:db8::ffff:0000:1  Incorrect. The 0000 can be shortened to just 0.

B. 2001:0db8:0:ffff::1  Incorrect. The multiple octets of 0000 are shortened to :: and the single octet of 0 is shortened to just 0.

C. 2001:0db8::ffff:0:0001  Incorrect. The final octet can be shortened from 0001 to 1.

D. 2001:db8::ffff:0:1 Correct. This is the shortened version of the address.

# What is WiFi?

Wireless networking is a popular method of connecting corporate and home systems because of the ease of deployment and relatively low cost. It has made networking more versatile than ever before. Workstations and portable systems are no longer tied to a cable but can roam freely within the signal range of the deployed wireless access points. However, with this freedom comes additional vulnerabilities.

Wi-Fi range is generally wide enough for most homes or small offices, and range extenders may be placed strategically to extend the signal for larger campuses or homes. Over time the Wi-Fi standard has evolved, with each updated version faster than the last.  

In a LAN, threat actors need to enter the physical space or immediate vicinity of the physical media itself. For wired networks, this can be done by placing sniffer taps onto cables, plugging in USB devices, or using other tools that require physical access to the network. By contrast, wireless media intrusions can happen at a distance.
![[EDU-ELCC-70245b-What_is_Wifi-techart-v06.jpg]]

# Security of the Network 

TCP/IP’s vulnerabilities are numerous. Improperly implemented TCP/IP stacks in various operating systems are vulnerable to various 

>[!DoS/DDoS attacks]-
>The prevention of authorized acccess to resources or the delaying of time-critical operations. (Time critical can be milliseconds or it may be hours, depending upon the service provided). NIST SP 800-27 REV. A 

>[!fragment attacks]- 
>In a fragmenti attack, an attacker fragments traffic in such a way that a system is unable to put data packets back togheter. 

>[!oversized packet attacks]-
>Purposely sending a network packet that is larger than expected or larger than can be handled by the receiving system, causing the receiving system to fail unexpectedly. 

>[!Spoofing attacks]-
>Faking the sending address of a transmission to gain illegal entry into a secure system. CNSSI 4009-2015 


>[!man-in-the-middle attacks]-
>An attack where the adversary positions himself between the user and the systems so that he can intercept and alter data traveling between them. NISTIR 7711

TCP/IP (as well as most protocols) is also subject to passive attacks via monitoring or sniffing. Network monitoring, or sniffing, is the act of monitoring traffic patterns to obtain information about a network. ![[EDU-ELCC-70245c-techart-Security_Network-v05.jpg]]

[diagram of network with internet, router and firewall highlighted in blue]


# Ports and Protocols (Applications/Services)

There are physical ports that you connect wires to and logical ports that determine where the data/traffic goes. 


[Physical Ports]()
Physical ports are the ports on the routers, switches, servers, computers, etc. that you connect the wires, e.g., fiber optic cables, Cat5 cables, etc., to create a network.

_Click on each tab to learn more._

[Logical Ports]()

When a communication connection is established between two systems, it is done using ports. A logical port (also called a socket) is little more than an address number that both ends of the communication link agree to use when transferring data. Ports allow a single IP address to be able to support multiple simultaneous communications, each using a different port number. In the Application Layer of the TCP/IP model (which includes the Session, Presentation, and Application Layers of the OSI model) reside numerous application- or service-specific protocols. Data types are mapped using port numbers associated with services. For example, web traffic (or HTTP) is port 80. Secure web traffic (or HTTPS) is port 443. Table 5.4 highlights some of these protocols and their customary or assigned ports. You’ll note that in several cases a service (or protocol) may have two ports assigned, one secure and one insecure. When in doubt, systems should be implemented using the most secure version as possible of a protocol and its services.

-   Well-known ports (0–1023): These ports are related to the common protocols that are at the core of the Transport Control Protocol/Internet Protocol (TCP/IP) model, Domain Name Service (DNS), Simple Mail Transfer Protocol (SMTP), etc.
-   Registered ports (1024–49151): These ports are often associated with proprietary applications from vendors and developers. While they are officially approved by the Internet Assigned Numbers Authority (IANA), in practice many vendors simply implement a port of their choosing. Examples include Remote Authentication Dial-In User Service (RADIUS) authentication (1812), Microsoft SQL Server (1433/1434) and the Docker REST API (2375/2376).
-   Dynamic or private ports (49152–65535): Whenever a service is requested that is associated with well-known or registered ports, those services will respond with a dynamic port that is used for that session and then released.

# Secure Ports

Some network protocols transmit information in clear text, meaning it is not encrypted and should not be used. Clear text information is subject to network sniffing. This tactic uses software to inspect packets of data as they travel across the network and extract text such as usernames and passwords. Network sniffing could also reveal the content of documents and other files if they are sent via insecure protocols. The table below shows some of the insecure protocols along with recommended secure alternatives.

_Click each insecure port on the left to discover why it is insecure and why the corresponding secure alternative port is preferred._ 


| **Insecure Port** | **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | **Protocol**                          | **Secure Alternative Port** | **Protocol**                                 |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- | --------------------------- | -------------------------------------------- |
| 21 - FTP          | Port 21, File Transfer Protocol (FTP) sends the username and password using plaintext from the client to the server. This could be intercepted by an attacker and later used to retrieve confidential information from the server. The secure alternative, SFTP, on port 22 uses encryption to protect the user credentials and packets of data being transferred.                                                                                                                                                                                                                             | File Transfer Protocol                | 22* - SFTP                  | Secure File Transfer Protocol                |
| 23 - Telnet       | Port 23, telnet, is used by many Linux systems and any other systems as a basic text-based terminal. All information to and from the host on a telnet connection is sent in plaintext and can be intercepted by an attacker. This includes username and password as well as all information that is being presented on the screen, since this interface is all text. Secure Shell (SSH) on port 22 uses encryption to ensure that traffic between the host and terminal is not sent in a plaintext format.                                                                                     | Telnet                                | 22* SSH                     | Secure Shell                                 |
| 25 - SMTP         | Port 25, Simple Mail Transfer Protocol (SMTP) is the default unencrypted port for sending email messages. Since it is unencrypted, data contained within the emails could be discovered by network sniffing. The secure alternative is to use port 587 for SMTP using Transport Layer Security (TLS) which will encrypt the data between the mail client and the mail server.                                                                                                                                                                                                                  | Simple Mail Transfer Protocol         | 587 SMTP                    | SMTP with TLS                                |
| 37 - TIME         | Port 37, Time Protocol, may be in use by legacy equipment and has mostly been replaced by using port 123 for Network Time Protocol (NTP). NTP on port 123 offers better error-handling capabilities, which reduces the likelihood of unexpected errors.                                                                                                                                                                                                                                                                                                                                        | Time Protocol                         | 123 - NTP                   | Network Time Protocol                        |
| 53 - DNS          | Port 53, Domain Name Service (DNS), is still used widely. However, using DNS over TLS (DoT) on port 853 protects DNS information from being modified in transit.                                                                                                                                                                                                                                                                                                                                                                                                                               | Domain Name Service                   | 853 - DoT                   | DNS over TLS (DoT)                           |
| 80 - HTTP         | Port 80, HyperText Transfer Protocol (HTTP) is the basis of nearly all web browser traffic on the internet. Information sent via HTTP is not encrypted and is susceptible to sniffing attacks. HTTPS using TLS encryption is preferred, as it protects the data in transit between the server and the browser. Note that this is often notated as SSL/TLS. Secure Sockets Layer (SSL) has been compromised is no longer considered secure. It is now recommended for web servers and clients to use Transport Layer Security (TLS) 1.3 or higher for the best protection.                      | Hyper Text Transfer Protocol          | 443 - HTTPS                 | http ON SSL/TLS                              |
| 143 - IMAP        | Port 143, Internet Message Access Protocol (IMAP) is a protocol used for retrieving emails. IMAP traffic on port 143 is not encrypted and susceptible to network sniffing. The secure alternative is to use port 993 for IMAP, which adds SSL/TLS security to encrypt the data between the mail client and the mail server.                                                                                                                                                                                                                                                                    | Internet Message Access Protocol      | 993 - IMAP                  | IMAP for SSL/TLS                             |
| 161/162 - SNMP    | Ports 161 and 162, Simple Network Management Protocol, are commonly used to send and receive data used for managing infrastructure devices. Because sensitive information is often included in these messages, it is recommended to use SNMP version 2 or 3 (abbreviated SNMPv2 or SNMPv3) to include encryption and additional security features. Unlike many others discussed here, all versions of SNMP use the same ports, so there is not a definitive secure and insecure pairing. Additional context will be needed to determine if information on ports 161 and 162 is secured or not. | Simple Network Management Protocol    | 161/162 SNMP                | SNMP v3                                      |
| 445 - SMB         | Port 445, Server Message Block (SMB), is used by many versions of Windows for accessing files over the network. Files are transmitted unencrypted, and many vulnerabilities are well-known. Therefore, it is recommended that traffic on port 445 should not be allowed to pass through a firewall at the network perimeter. A more secure alternative is port 2049, Network File System (NFS). Although NFS can use encryption, it is recommended that NFS not be allowed through firewalls either.                                                                                           | Server Message Block                  | 2049 - NFS                  | Network File System                          |
| 389 - LDAP        | Port 389, Lightweight Directory Access Protocol (LDAP), is used to communicate directory information from servers to clients. This can be an address book for email or usernames for logins. The LDAP protocol also allows records in the directory to be updated, introducing additional risk. Since LDAP is not encrypted, it is susceptible to sniffing and manipulation attacks. Lightweight Directory Access Protocol Secure (LDAPS) adds SSL/TLS security to protect the information while it is in transit.                                                                             | Lightweight Directory Access Protocol | 636 - LDAPS                 | Lightweight Directory Access Protocol Secure |


# SYN, SYN-ACK, ACK Handshake

## VIDEO AckHandShake.mkv


Transcript
Narrator: Between the client and the server, there is a system for synchronizing and acknowledging any request that is known as a three-way handshake. This handshake is used to establish a TCP connection between two devices. Here, we will take a simplified look at how communications are established to a web server. Depending on the exact protocol, there may be additional connection negotiation taking place. First, the client sends synchronization (SYN) packet to the web server’s port 80 or 443. This is a request to establish a connection. The web server replies to the SYN packet with an acknowledgement known as a SYN/ACK. Finally, the client acknowledges the connection with an acknowledgement (ACK). At this point, the basic connection is established, and the client and host will further negotiate secure communications over that connection.

# Matching Ports with Their Secure Counterparts

Which of the following protocols is a secure alternative to using telnet? (D4, L4.1.2) 

 A. HTTPS
Incorrect. HyperText Transfer Protocol Secure is the secure alternative for HTTP and uses SSL/TLS for securing website communications.

 B. LDAPS
Incorrect. Lightweight Directory Access Protocol Secure (LDAPS) is the secure alternative for Lightweight Directory Access Protocol (LDAP) and is used to exchange directory information in a secured protocol.

 C. SFTP
Incorrect. Secure File Transfer Protocol (SFTP) is the secure alternative to FTP and is used to transfer files.

 D. SSH
Correct. Secure Shell (SSH) is the secure alternative to telnet as it encrypts all traffic between the host and remote user.


