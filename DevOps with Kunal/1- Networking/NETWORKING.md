<h1 align="center"> Networking </h1>

<h3 align="center"> The Internet: A Network of Networks </h3>

### Computer Network & Internet
In simple terms (layman term), computer network means computers connected to each other with cables or wireless radio and a sort of group of computers is formed and 
these different groups(network of computers) are connected and are termed as the Internet(a network of computer networks) .


### ***Protocols***
A set of rules governing the exchange or transmission of data between devices or
the rules for exchange of data are called ***Protocols*** . 
Here a question may arise in your mind, why do we need protocols?. If yes, then here is the **answer**. 
Suppose, you made an application and set some rules for the communication with other applications, but some other person made other rules for communicating.
So, due to this issue, communication is not feasible. Therefore, a set of standerd rules is important to have, which is written by 
[***Internet Society Organization***](https://www.internetsociety.org/learning/?gclid=CjwKCAiA55mPBhBOEiwANmzoQollWESh4rtBH7KNA-VvlJ5_f0RZ4ukLkznK23Y2R-RWM4DOYvlT8BoCj10QAvD_BwE).

Some common Protocols are 
 - TCP (Transmission Control Protocol)
 - UDP (User Datagram Protocol)
 - HTTP (HyperText Transfer Protocol)
 
 ### ***TCP***
 The Transmission Control Protocol is a protocol that ensures that **100%** of data reaches the intended destination and
is not corrupted along the way.
So, if you want a person to get something completely, then you are going to use this protocol.
 
 ### ***UDP*** 
 User Datagram Protocol (UDP) does not ensure that data reaches the destination, and that it remains incorrupt.
 When it doesn't matter whether **100%** data is reaching to the intended user, you use UDP like in case of **Video Conferencing**.
 
 ### ***HTTP***
HyperText Transfer Protocol (HTTP) is a web protocol that defines the
format of messages to be exchanged between the web clients. e.g., web browsers
and web servers and what action is to be taken in response to the message, or in other terms,
It is the rule by which your data is being transferred between a client and server.
This is used by ***World Wide Web***.
  - World Wide Web is collection of all the information/pages/documents which are interlinked, meaning 
    we can go from one page to second, second to third and so on.
 
 With the following protocols, we have established a communication system. Computer send messages to one another. (These messages are made up of ones and zeros, bits). However, instead of sending the whole message (that could be more than trillion's of bits) at once, information/message is broken down into smaller units called ***Packets***
 Now, We have protocols and Packet is ready for sending. We need some sort of addressing via which packet(smaller unit of message) has to be sent to a certain application on a certain end system (Devices connected to Internet also called as Edge Systems like Mobile Phone, Desktop Computers etc). So, here comes the role of **Addressing**. 
 
 One more thing to mention here is ***Network Edge*** which is collection of end systems. Note, devices that relay messages like router are not part of Network Edge.
 
 ### ***IP Address***
 Every device that is connected to the Internet has an address called an ‘IP
Address’ which is much like a mailing address, means a 
unique address of the modem (provided by your Internet service provider) called **Global IP** .
You can check your computer *IP address* using ``` curl ifconfig.me -s ``` in your command line interface. 
There can be multiple devices connected to the modem. Modem will provide IP address to each of the devices connected to that modem,
using DHCP (Dynamic Host Configration Protocal). Each device can have lot of applications, so exactly which application is requesting the data is determined by ***PORTS***
<h3 align="center"> IP addresses identify end systems but ports identify an application on the end system </h3>
 

 
Data needs to be transmitted from one end system to another over a medium. 
There are two kinds of media
 - Guided
 - Unguided
 
1- Guided: A medium in which the signal is transported on a
defined pathway is called guided, like Fibre Optics.

2- Unguided: Means of transmission that are not bound by a confined pathway are called
unguided media, such as radio waves.

Now before we go further into technical details, lets review about data transmission over network and the network types
how is data transfered?(a brief overview)
Generally this happens when a Device Made a request. Request will go to the router.
 
From ***Router --> Inter Service Provider --> Internet***

>> When you send a WhatsApp message like "good morning" it is not sent as it is in one go in the vast ocean of internet, instead it happens in chunks.
Your data is transferred into segments, packets and frames(you will learn more about it in detail ). Same thing happens when you load a webpage,
individual calls are made for each "chunk" of data.
Every device that can be connected has an IP address. An IP address is in the form of X.X.X.X. each X can contain 0-255 no.s. this tells the internet, to where send and receive the data. Your "good morning" message will be sent to your friend only if the internet know which IP address
he/she has. But wait? how does the internet knows which application to send to ? it is not like you send a whatsapp message and it has sent in
your friend email,is it? for that there are port numbers, which tells which application this "good morning" message has to be sent.Ports are 16 bit
no.s and some are already reserved. forexample:- port no. 80 is reserved for http.
Now this is one final problem , the problem of sequence. when you send "good morning" why doesnt the data is tranfered as "morning gdoo", how
does the sequence of those data packets is maintained? the answer is sequence no.s. they maintain the sequence of those data packets to be transferred.
So there it is a simple overview of how your simple message in form of data is transferred form one computer to another.
You will learn more in detail when u will study network models like OSI model and TCP/IP model.


But wait, now you know how does data travels in this "network" thing, but what exactly is a computer network who are these connected with wires?
the answer is CABLES, CABLES, CABLES everyone is connected with cables around the globe. Checkout the website submarinecable.com .
Now lets talk about how this network is arranged there are basicly three type of network connection LAN, MAN and WAN , which are explained below:-
### Local Area Network(LAN)
It is a computer network  that links devices within a building or group of adjacent buildings, especially one with a radius of less than 1 km. House is network(HAN) and personal area network(PAN) come under this category.
 
### Metropolitan Area Network(MAN)
A metropolitan area network (MAN) is a computer network that connect computers within a metropolitan area, which could be a single large city, multiple cities and towns, or any given large area with multiple buildings. It generally ranges from 5 to 50 km.

### Wide Area Network(WAN)
A wide area network ( WAN) is a telecommunication's network that extends over a large geographical area for the primary purpose of computer networking.
A good example of wide area network is the airtel.
And the internet is a collection of all these networks.
However there is one special kind of network which we have not reviewed yet and it is called Virtual Private Network(VPN)

VPN (Virtual Private Network) : VPN or the Virtual Private Network is a private WAN
(Wide Area Network) built on the internet. It allows the creation of a secured tunnel
(protected network) between different networks using the internet (public network). By
using the VPN, a client can connect to the organization’s network remotely.
>> Advantages of VPN :
1. VPN is used to connect offices in different geographical locations remotely and is
cheaper when compared to WAN connections.
2. VPN is used for secure transactions and confidential data transfer between
multiple offices located in different geographical locations.
3. VPN keeps an organization’s information secured against any potential threats or
intrusions by using virtualization.
4. VPN encrypts the internet traffic and disguises the online identity.
>> Types of VPN :
1. Access VPN: Access VPN is used to provide connectivity to remote mobile users and
telecommuters. It serves as an alternative to dial-up connections or ISDN (Integrated
Services Digital Network) connections. It is a low-cost solution and provides a wide
range of connectivity.
2. Site-to-Site VPN: A Site-to-Site or Router-to-Router VPN is commonly used in large
companies having branches in different locations to connect the network of one office to
another in different locations. There are 2 sub-categories as mentioned below:
3. Intranet VPN: Intranet VPN is useful for connecting remote offices in different
geographical locations using shared infrastructure (internet connectivity and servers)
with the same accessibility policies as a private WAN (wide area network).
4. Extranet VPN: Extranet VPN uses shared infrastructure over an intranet, suppliers,
customers, partners, and other entities and connects them using dedicated connections.

### Now , lets talk about network topologies before we jump into osi model:-

Network Topology : Network topology specifies the layout of a computer network. It shows how devices and cables are connected to each other. Types of Network Topology are as follows:-
### Bus :
1. Bus topology is a network topology in which all the nodes are connected to a
single cable known as a central cable or bus.
2. It acts as a shared communication medium, i.e., if any device wants to send the
data to other devices, then it will send the data over the bus which in turn sends
the data to all the attached devices.
3. Bus topology is useful for a small number of devices.
4. As if the bus is damaged then the whole network fails.
### Ring :
1. Ring topology is a network topology in which nodes are exactly connected to two
or more nodes and thus, forming a single continuous path for the transmission.
2. It does not need any central server to control the connectivity among the nodes.
3. If the single node is damaged, then the whole network fails.
4. Ring topology is very rarely used as it is expensive, difficult to install and manage.
5. Examples of Ring topology are SONET network, SDH network, etc
### Star :
1. Star topology is a network topology in which all the nodes are connected to a single device known as a central device.
2. Star topology requires more cable compared to other topologies.
Therefore, it is more robust as a failure in one cable will only disconnect aspecific computer connected to this cable.
3. If the central device is damaged, then the whole network fails.
4. Star topology is very easy to install, manage and troubleshoot. It iscommonly used in office and home networks.
### Tree :
1. Tree topology is a combination of star and bus topology. It is also known as theexpanded star topology.
2. In tree topology, all the star networks are connected to a single bus.
3. Ethernet protocol is used in this topology.
4. In this, the whole network is divided into segments known as star networks whichcan be easily maintained. If one segment is damaged, there is no effect on othersegments.
5. Tree topology depends on the "main bus," and if it breaks, then the whole network gets damaged.
### Mesh :
1. Mesh topology is a network topology in which all the nodes are individually connected to other nodes.
2. It does not need any central switch or hub to control the connectivity among the nodes.
3. Mesh topology is categorized into two parts: 
 Fully connected mesh topology:
In this topology, all the nodes are connected to each other.
 Partially connected
mesh topology: In this topology, all the nodes are not connected to each other.
4. It is robust as a failure in one cable will only disconnect the specified computer connected to this cable.
5. Mesh topology is rarely used as installation and configuration are difficult when connectivity gets more.
6. Cabling cost is high as it requires bulk wiring.
#### Hybrid :
1. A hybrid topology is a combination of different topologies to form a resulting topology.
2. If star topology is connected with another star topology, then it remains a star topology. If star topology is connected with different topology, then it becomes Hybrid topology.
3. It provides flexibility as it can be implemented in a different network environment.

 ### OSI Model(Open System Interconnections) (Imp) : 
It is a network architecture model based
on the ISO standards. It is called the OSI model as it deals with connecting the systems
that are open for communication with other systems. The OSI model has seven layers.
- Open Systems Interconnection Model, developed by International Organization for Standardization(ISO). 
- It is a *reference model* for how applications communicate over the n/w. 
- It is like a universal language for computer networking.
- It consists of 7 layers and summarized briefly as below
  1. Physical Layer
  2. DataLink Layer
  3. Network Layer
  4. Transport Layer
  5. Session Layer
  6. Presentation Layer
  7. Application Layer
 
***Application Layer***
 It is the top most layer in OSI model. It is a software layer which is implemented by n/w applications. These applications produce the data which has to be transferred over the n/w. And this layer serves as a window for those application services to access the network and for displaying the received information to the user. Also known as *Desktop Layer*
  Eg: Browsers, Twitter and all similar applications

***Presentation Layer***
 It is also called as Translation layer. The data from the application layer is extracted here and manipulated as per the required format to transmit over the network. 
The functions of the presentation layer are 
1. Translation: Converting our ascii data into interchangeable binary data(ASCII to EBCDIC).
2. Encryption/ Decryption: Encrypts our data for abstraction. And Decrypts the encrypted data.
3. Compression: Reduces the number of bits that need to be transmitted on the network.

***Session Layer***
 - It is responsible for the establishment of connection, maintenance of sessions, use and termination of connections authentication, authorizations and security. (*Session Establishment, Maintenance & Termination*)
 - It enables two systems to start sending and receiving of data in half-duplex or full-duplex modes & followed by the termination of connected sessions. (*Dialog Controller*)
-  It also avoids data loss by adding checkpoints called synchronization points into the data.. (*Synchronization*)

***Transport Layer***
- The data received from the Application layer through presentation and session layers is changed or divided into the small data units called Segments (Process is Segmentation). Responsible for end to end delivery of the complete message. And transport layer also provides the acknowledgement of successful data transmission and re-transmits the data if an error is found. 
- At sender side, Transport layer receives the formatted & encrypted data from the upper layers, performs Segmentation and also implements Flow & Error Control to ensure proper data transmission. And for every segment, it will also add Source Portno, Destination Portno (Known or Default port of Receiver's app like 80 for web apps), Sequence Number in its header and forwards the segmented data to N/w layer.
- At receivers side, TL reads the portnumber from its header and forwards the data to respective application. It also performs reassembling the segmented data based on sequence numbers.
- So, Functions of TL are Segmentation & Reassembling, Service Point or Port Addressing (To deliver the messafe to correct app or process by port address in the header)
- It provides both connection oriented and connection less services.
- TL is operated by OS and it is a part of the OS that communicates with upper layers or Application layer by making system calls.
- This also termed as Heart of OSI Model.

**Network Layer**
- The network layer works for the transmission of data from one host to the other located in different networks. It also takes care of packet routing i.e. selection of the shortest path to transmit the packet, from the number of routes available.
-  The sender & receiver’s IP addresses are placed in the header by the network layer.
-  Functions of the Network layer are Routing (The network layer protocols determine which route is suitable from source to destination) & Logical Addressing or IP addressing (In order to identify each device on internetwork uniquely, the network layer defines an addressing scheme. Through Ip addresses it can distinguish each device uniquely and universally.)
-  Segments in N/w Layer is called as Packets(Segments encoded with n/w layer headers like adding source IP, Destination Ip )

**Data Link Layer**
- The data link layer is responsible for the node-to-node delivery of the message. The main function of this layer is to make sure data transfer is error-free from one node to another, over the physical layer.
- The data unit in the DLL is a frame which can be accomplished by attaching special bit patterns to beginning and end of the frame. DLL also encapsulates Sender and Receiver’s MAC address in the header. 

- Whenever a packet is transferred on the network based on the IP address it will find network and from there for delivering to the correct device it need a another unique address where MAC address comes to the picture.
- The MAC address(12 digit alpha numeric) of a computer is the unique physical address of the network device, and it never changes. It is assigned with something based on where the computer is made and it exists for the lifetime of that network device.
- But we can get a question like Why do we need a MAC address when we have a private IP address for each device assigned by routers using DHCP?
Eg: Think of private Ip address as a shortcut on your computer. When a phone joins a network, it presents itself as d8:8n:v8 (example)Mac address, the DHCP server will then generate a private IP for it, or use one that's been reserved for that MAC (192.168.56.11 for example). So now when you communicate with 192.168.56.11, you're actually just communicating with d8:8n:v8 (Here Receiver’s MAC address is obtained by placing an ARP(Address Resolution Protocol) request onto the wire asking “Who has that IP address?” and the destination host will reply with its MAC address). Private IP addresses are not unique, MAC addresses are unique. 
- Data Link Layer is divided into two sublayers called Logical Link Control (LLC) & Media Access Control (MAC).
- Functions are 
 1. Framing (Provides a way for sender to transmit a set of bits to the receiver by adding special bit patterns to the beginning and end of the frames to identify their boundaries).
 2. Physical Addressing (After creating frames, the Data link layer adds physical addresses (MAC address) of the sender and/or receiver in the header of each frame. The DLL defines an addressing scheme called Physical addressing to identify device instead of n/w in logical addressing.)
 3. Error control: Data link layer provides the mechanism of error control in which it detects and retransmits damaged or lost frames.
 4. Flow Control: The data rate must be constant on both sides else the data may get corrupted thus, flow control coordinates the amount of data that can be sent before receiving acknowledgement.
 5. Access control: When a single communication channel is shared by multiple devices, the MAC sub-layer of the data link layer helps to determine which device has control over the channel at a given time.

**Physical Layer**
- The lowest layer responsible for the actual physical connection between the devices. The physical layer contains information in the form of bits. It is responsible for transmitting individual bits from one node to the next. When receiving data, this layer will get the signal received and convert it into 0s and 1s and send them to the Data Link layer, which will put the frame back together.
- Functions of the physical layer are 
  Bit synchronization: It provides the synchronization of the bits by providing a clock. Determining the boundary (start and end) of signal cell is known as bit or clock synchronization. Used to make sure that the signals sent from one host of the communication can be rightly decoded by the receiver.
  Bit rate control: It also defines the transmission rate i.e. the number of bits sent per second.
  Physical topologies: It specifies the way in which the different, devices/nodes are arranged in a network i.e. bus, star, or mesh topology.
  Transmission mode: It also defines the way in which the data flows between the two connected devices. The various transmission modes possible are Simplex, half-duplex and full-duplex.
- Hub, Repeater, Modem, Cables are Physical Layer devices. 

<h4 align="center">Application, Presentation & Session Layers are S/W layers. Transport Layer is Heart of OSI. N/W, Data Link & Physical Layers are H/w layers</h4>
Data Will be transferred from Application to Application similar to the below.
<p align="center"><img src="https://user-images.githubusercontent.com/70102577/151218840-02e1988d-680a-4a3a-bbb7-3d5ad27df80d.png" width=90% height=250px/></p>

### ***TCP/IP Model*** 
- Transmission Control Protocol/Internet Protocol.
- The OSI Model is just a reference/logical model. It was designed to describe the functions of the communication system by dividing the communication procedure into smaller and simpler components.
- Developed by ARPA Net(First internet n/w) in 1960s.
- TCP/IP is concise version of OSI and contains 5 layers.
1. Application Layer - User Interaction happens, It lies on the Devices
2. Transport Layer - 
3. Network Layer
4. DataLink Layer
5. Physical Layer

### ***Client Server Architecture***
<p align="center"><img src="https://user-images.githubusercontent.com/70102577/151224161-edb9d3b8-f661-453f-96c6-7824d9ec023b.png" width=90% height=250px/></p>
- An application with this architecture has the client where the user interacts and a server to send the data to client when it is requested. Each client and server contains processes. These processes communicate with each other.
- Server will high availablity and performance to serve the requests from the clients.
- Clients will be interactive with the users and send requests to the server and serve the response from server to the client in an understandable and interactive way. 
- Collection of servers are known as Data Centers.

### ***Peer to Peer Architecture***
- This architecture consists of a decentralized network of peers - nodes that are both clients and servers. P2P networks distribute the workload between peers, and all peers contribute and consume resources within the network without the need for a centralized server.
- Eg: Bit Torrent downloads using P2P transfers

### ***Network Devices***
1. Repeater – A repeater operates at the physical layer. Its job is to regenerate the signal over the same network before the signal becomes too weak or corrupted so as to extend the length to which the signal can be transmitted over the same network. An important point to be noted about repeaters is that they do not amplify the signal. When the signal becomes weak, they copy the signal bit by bit and regenerate it at the original strength. It is a 2 port device. 


2. Hub –  A hub is basically a multiport repeater. A hub connects multiple wires coming from different branches, for example, the connector in star topology which connects different stations. Hubs cannot filter data, so data packets are sent to all connected devices.  In other words, the collision domain of all hosts connected through Hub remains one.  Also, they do not have the intelligence to find out the best path for data packets which leads to inefficiencies and wastage. 

*Types of Hub*
a. Active Hub:- These are the hubs that have their own power supply and can clean, boost, and relay the signal along with the network. It serves both as a repeater as well as a wiring center. These are used to extend the maximum distance between nodes.

b. Passive Hub :- These are the hubs that collect wiring from nodes and power supply from the active hub. These hubs relay signals onto the network without cleaning and boosting them and can’t be used to extend the distance between nodes.

c. Intelligent Hub :- It works like active hubs and includes remote management capabilities. They also provide flexible data rates to network devices. It also enables an administrator to monitor the traffic passing through the hub and to configure each port in the hub.


3. Bridge – A bridge operates at the data link layer. A bridge is a repeater, with add on the functionality of filtering content by reading the MAC addresses of source and destination. It is also used for interconnecting two LANs working on the same protocol. It has a single input and single output port, thus making it a 2 port device.

*Types of Bridges*
Transparent Bridges:- These are the bridge in which the stations are completely unaware of the bridge’s existence i.e. whether or not a bridge is added or deleted from the network, reconfiguration of the stations is unnecessary. These bridges make use of two processes i.e. bridge forwarding and bridge learning.
Source Routing Bridges:- In these bridges, routing operation is performed by the source station and the frame specifies which route to follow. The host can discover the frame by sending a special frame called the discovery frame, which spreads through the entire network using all possible paths to the destination.

4. Switch – A switch is a multiport bridge with a buffer and a design that can boost its efficiency(a large number of ports imply less traffic) and performance. A switch is a data link layer device. The switch can perform error checking before forwarding data, which makes it very efficient as it does not forward packets that have errors and forward good packets selectively to the correct port only.  In other words, the switch divides the collision domain of hosts, but broadcast domain remains the same. 
  
5. Routers – A router is a device like a switch that routes data packets based on their IP addresses. The router is mainly a Network Layer device. Routers normally connect LANs and WANs together and have a dynamically updating routing table based on which they make decisions on routing the data packets. Router divide broadcast domains of hosts connected through it.

6. Gateway – A gateway, as the name suggests, is a passage to connect two networks together that may work upon different networking models. They basically work as the messenger agents that take data from one system, interpret it, and transfer it to another system. Gateways are also called protocol converters and can operate at any network layer. Gateways are generally more complex than switches or routers. Gateway is also called a protocol converter. 

7. Brouter – It is also known as the bridging router is a device that combines features of both bridge and router. It can work either at the data link layer or a network layer. Working as a router, it is capable of routing packets across networks, and working as the bridge, it is capable of filtering local area network traffic. 

8. NIC – NIC or network interface card is a network adapter that is used to connect the computer to the network. It is installed in the computer to establish a LAN.  It has a unique id that is written on the chip, and it has a connector to connect the cable to it. The cable acts as an interface between the computer and router or modem. NIC card is a layer 2 device which means that it works on both physical and data link layer of the network model. 
<p align="center"><img src="https://user-images.githubusercontent.com/70102577/151415927-d5430a05-8a88-4973-b015-c66658a5d51b.png" width=90% height=250px/></p>


### **_Ports_**

- It tells us which application we are working with.
- Port Numbers are 16-bit numbers. (2^16 = 65000 ports are available in a system)
- Port Numbers are useful to identify the process or applications running on the device.

- _Ephemeral Ports:_&nbsp; Ephemeral ports are communication endpoints of a transport layer protocol of TCP/IP & these are temporary or short-lived ports used for short period of time. After communication is terminated, the port becomes available for use in another session.

- All the HTTP requests and responses are especially processed and transmitted on port 80.
  0-1023 - Reserved Ports
  1024-49152 - Application Ports
  49153 - 65535 - Usable ports (Ephemeral)

  1 mbps = 10,00,000 bits/s
  1gbps = 10^9 bits/s
  1kbps = 1000 bits/s

### **_Sockets_**

- A socket is one endpoint of a two-way communication link between two programs running on the network.
- They acts as interface to connect with two-way communication network and allows processes to communicate with each other.
- Especially used in client-server applications that allow for communication between applications.
- A socket is created by concatenating the IP number of a system and a software port number by which application to application communication is possible.

### ***Protocols***
A set of rules governing the transmission of data between devices Or The rules for the exchange of data are called Protocols.

***Web Protocols***
**TCP/IP Protocols**
- HTTP
- DHCP
- FTP
- SMTP
- POP3 & IMAC
- SSH
- VNC

- TELNET - Manage an account or device remotely. port 23
- UDP - Stateless Connection less protocol

***MiddleBoxes***
- A middleBoxes is a networking devices that transforms, inspects, filter and manipulates traffic for purposes other than packet forwarding.
**Types -**
 **1. Firewall**
- Firewall as you may have heard filter out 18 packets bases on various rules like Addresses, modifying packets, Port no., flags, protocols.
- **Stateless Firewall** - Will not maintain state even if it sees the packets
- **Statefull Firewall** - Wil maintain state after carefully watching state. It's in Network Layer and transport layer also.
**2. Network Address Translation(NAT)**
- NAT is a method of mapping an IP address space into another by modifying network address information in the IP header of packets while they are on transit across a traffic routing device.
- IT modifies the IP to slow down the consumption of IP addresses.
