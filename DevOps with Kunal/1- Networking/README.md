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
    
  
  You may have a doubt that how one computer determine that this is the computer to which I was sending data.
  So, here comes the role of **IP addresses**. 
 
 ### ***IP Address***
 Every device that is connected to the Internet has an address called an ‘IP
Address’ which is much like a mailing address means a 
unique address of the modem (provided by your Internet service provider) called **Global IP** .
You can check your computer *IP address* using ``` curl ifconfig.me -s ``` in your command line interface. 
There can be multiple devices connected to the modem. Modem will give IP address to each of device which is connected to that modem,
using DHCP (Dynamic Host Configration Protocal).
 
 How we will get the searched file in laymans term. 
 Device Made a request, it will go to the router. From router --> Inter Service Provider --> Internet
 
