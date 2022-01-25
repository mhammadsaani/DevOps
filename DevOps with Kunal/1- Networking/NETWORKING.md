<h1 align="center"> Networking </h1>

<h3 align="center"> The Internet: A Network of Networks </h3>

### Computer Network & Internet
In simple term (layman term), computer network means computer connected to each other with cables or wireless radio and a sort of group of computers is formed and 
these different groups(network of computers) are connected and are termed as Internet(a network of computer networks) .


### ***Protocols***
A set of rules governing the exchange or transmission of data between devices Or
The rules for exchange of data are called ***Protocols*** . 
Here a question may arise in your mind, why we need protocols?. If yes, then here is the **answer**. 
Suppose, you made an application and set some rules for communicating this application with other application but some other person made other rules for communicating.
So, due to this issue, communication is not feasible. Therefore, a set of standerd rules is important to have, which is written by 
[***Internet Society Organization***](https://www.internetsociety.org/learning/?gclid=CjwKCAiA55mPBhBOEiwANmzoQollWESh4rtBH7KNA-VvlJ5_f0RZ4ukLkznK23Y2R-RWM4DOYvlT8BoCj10QAvD_BwE).

Some common Protocols are 
 - TCP (Transmission Control Protocol)
 - UDP (User Datagram Protocol)
 - HTTP (Hyper Text Transfer Protocol)
 
 ### ***TCP***
 The Transmission Control Protocol is a protocol that ensures that **100%** of data reaches the intended destination and
is not corrupted along the way
So, if you want a person to get something completely, then you are going to use this protocol.
 
 ### ***UDP*** 
 User Datagram Protocol (UDP) does not ensure that data reaches the destination or not and that it remains incorrupt.
 When you do not care if **100%** data is reaching to your friend or not, you use UDP like in case of **Video Conferencing**.
 
 ### ***HTTP***
HyperText Transfer Protocol (HTTP) is a web protocol that defines the
format of messages to be exchanged between web clients, e.g., web browsers
and web servers and what action is to be taken in response to the message. Or in other terms,
It is the rule via which your data is being transferred between a client and server.
This is used by ***World Wide Web***.
  - World Wide Web is collection of all the information/pages/documents which are interlinked meaning 
    we can go from one page to second, second to third and so on.
 
 Following protocols, we have established a communication system. Computers send messages to one another. (These messages are made up of ones and zeros, bits). However, instead of sending the whole message (that could be more than trillion bits) at once, information/message is broken down into smaller units called ***Packets***
 Now, Packet is ready for sending and packet(smaller unit of message) has to be addressed to a certain application on a certain end system (Devices connected to Internet also called as Edge Systems like Mobile Phone, Desktop Computers etc). So, here comes the role of **Addressing**. 
 
 One more thing to mention here is ***Network Edge*** which is collection of end systems. Note, devices that relay messages like router are not part of Network Edge.
 
 ### ***IP Address***
 Every device that is connected to the Internet has an address called an ‘IP
Address’ which is much like a mailing address means a 
unique address of the modem (provided by your Internet service provider) called **Global IP** .
You can check your computer *IP address* using ``` curl ifconfig.me -s ``` in your command line interface. 
There can be multiple devices connected to the modem. Modem will give IP address to each of device which is connected to that modem,
using DHCP (Dynamic Host Configration Protocal). Each device can have lot of applications, so exactly which application is requesting the data is determined by ***PORTS***
<h3 align="center"> IP addresses identify end systems but ports identify an application on the end system </h3>
 
 How we will get the searched file in laymans term. 
 Device Made a request, it will go to the router.
 
 From ***Router --> Inter Service Provider --> Internet***
 
Data needs to be transmitted from one end system to another over a medium. 
There are two kinds of media
 - Guided
 - Unguided
1- Guided: A medium in which the signal is transported on a
defined pathway is called guided like Fibre Optics
2- Unguided: Means of transmission that are not bound by a confined pathway are called
unguided media, such as radio waves.

Now before we go further into technical details lets reviw about data trasmission over network and the network types
how is data transfered?(a brief overview)
>> when u send a wattsapp message like "good morning" it is not sent as it is in one go in the vast ocean of internet, instead it happens in chunks
ur data is transfered into segments, packates and frames(you will learn more about it in detail ). same thing happens when u load a webpage
individual calls are made for each "chunk" of data.
Every device that can be connected has an IP address.An IP address is in the form of X.X.X.X. each X can contain 0-255 no.s. this address
will tell the internet to where send and recieve a data ur "good morning" message will be sent to ur friend only if the internet know which IP adress
he/she has. But wait? how does the internet knows which application to send to ? it is not like u send a wattsapp message and it has sent in
your friend email,is it? for that thier is port no.s which tells which application this "good morning" message has to be sent.Ports are 16 bit
no.s and some are already reserved. forexample:- port no. 80 is reservedd for http.
now this is one final problem , the problem of sequence. when u send "good morning" why doesnt the data is tranfered as "morning gdoo", how
does the sequence of those data packets is mainted? the answer is sequence no.s. they maintain the sequence of those data packets to be transferred
So there it is a simple overview of how your simple mesasage in form of data is tranferred form one computer to another.
You will learn more in detail when u will study network models like OSI model and TCP/IP model.


But wait now u know how does data travels in this "network" thing but what exactly is a computer network who are these connected with wires?
the ansawer is CABLES, CABLES , CABLES everyone is connected with cables around the globe.checkout the website submarinecable.com .
Now lets talk about how this network is arranged there are basicly three type of network connection LAN, MAN and WAN , which are explained below:-
### Local Area Network(LAN)
It is a computer network  that links devices within a building or group of adjacent buildings, especially one with a radius of less than 1 km.house are network(HAN) and personal area network(PAN) comes under this category.
 
### Metropolatian Area Network(MAN)
A metropolitan area network (MAN) is a computer network that connects computers within a metropolitan area, which could be a single large city, multiple cities and towns, or   any given large area with multiple buildings. It generally ranges from 5 to 50 km.

### Wide Area Network(WAN)
A wide area network ( WAN) is a telecommunications network that extends over a large geographical area for the primary purpose of computer networking.
A good example of wide area network is the aiertel.
And the internet is a collection of all these networks.
However there is one special kind of network which we have not reviewed yet and it is called Vitual Private Network(VPN)

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

Network Topology : Network topology specifies the layout of a computer network. Itshows how devices and cables are connected to each other.Types of Network Topology are as follows:-
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
4. Ring topology is very rarely used as it is expensive, difficult to install andmanage.
5. Examples of Ring topology are SONET network, SDH network, etc
### Star :
1. Star topology is a network topology in which all the nodes are connectedto a single device known as a central device.
2. Star topology requires more cable compared to other topologies.
Therefore, it is more robust as a failure in one cable will only disconnect aspecific computer connected to this cable.
3. If the central device is damaged, then the whole network fails.
4. Star topology is very easy to install, manage and troubleshoot. It iscommonly used in office and home networks.
### Tree :
1. Tree topology is a combination of star and bus topology. It is also known as theexpanded star topology.
2. In tree topology, all the star networks are connected to a single bus.
3. Ethernet protocol is used in this topology.
4. In this, the whole network is divided into segments known as star networks whichcan be easily maintained. If one segment is damaged, there is no effect on othersegments.
5. Tree topology depends on the "main bus," and if it breaks, then the wholenetwork gets damaged.
### Mesh :
1. Mesh topology is a network topology in which all the nodes are individuallyconnected to other nodes.
2. It does not need any central switch or hub to control the connectivity among thenodes.
3. Mesh topology is categorized into two parts: 
 Fully connected mesh topology:
In this topology, all the nodes are connected to each other.
 Partially connected
mesh topology: In this topology, all the nodes are not connected to each other.
4. It is robust as a failure in one cable will only disconnect the specified computerconnected to this cable.
5. Mesh topology is rarely used as installation and configuration are difficult whenconnectivity gets more.
6. Cabling cost is high as it requires bulk wiring.
#### Hybrid :
1. A hybrid topology is a combination of different topologies to form a resultingtopology.
2. If star topology is connected with another star topology, then it remains a startopology. If star topology is connected with different topology, then it becomes Hybrid topology.
3. It provides flexibility as it can be implemented in a different network environment.

 ### OSI Model(Open System Interconnections) (Imp) : 
It is a network architecture model based
on the ISO standards. It is called the OSI model as it deals with connecting the systems
that are open for communication with other systems. The OSI model has seven layers.
The principles used to arrive at the seven layers can be summarized briefly as below:



	
	
