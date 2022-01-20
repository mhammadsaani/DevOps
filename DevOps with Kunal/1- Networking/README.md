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
