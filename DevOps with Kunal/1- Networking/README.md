<h1 align="center"> Networking </h1>

### Computer Network & Internet
In simple term (layman term), computer network means computer connected together and a group of computers is formed and 
collected of these groups (connected computer networks) is termed as internet.

### ***Protocols***
The rules for sending particular data are called ***Protocols*** .
Here a question may arise in your mind, why we need protocols?. If yes, then here is the **answer**. 
Suppose, you made an application and set some rules for communicating this application with other application but some other person made other rules for communicating.
So, due to this issue, communication is not feasible. Therefore, a set of standerd rules is important to have, which is written by 
[***Internet Society Organization***](https://www.internetsociety.org/learning/?gclid=CjwKCAiA55mPBhBOEiwANmzoQollWESh4rtBH7KNA-VvlJ5_f0RZ4ukLkznK23Y2R-RWM4DOYvlT8BoCj10QAvD_BwE).

Some common Protocols are 
 - TCP (Transmission Control Protocol)
 - UDP (User Datagram Protocol)
 - HTTP (Hyper Text Transfer Protocol)
 
 ### ***TCP***
 This protocol ensures that **100%** of data will be reached to destination without being crupted. 
 So, if you want a person to get something completely, then you are going to use this protocol.
 
 ### ***UDP*** 
 When you do not care if **100%** data is reaching to your friend or not, you use UDP like in case of **Video Conferencing**.
 
 ### ***HTTP***
 It is the rule via which your data is being transferred between a client and server.
 This is used by ***World Wide Web***.
  - World Wide Web is collection of all the information/pages/documents which are interlinked meaning 
    we can go from one page to second, second to third and so on.
    
  
  You may have a doubt that how one computer determine that this is the computer to which I was sending data.
  So, here comes the role of **IP addresses**. 
 
 ### ***IP Address***
 IP address is a unique address of the modem (provided by your Internet service provider) called **Global IP** .
 You can check your computer *IP address* using ``` curl ifconfig.me -s ``` in your command line interface. 
 Everything that can communicate online has an IP address. There can be multiple devices connected to the modem.
 Modem will give IP address to each of device which is connected to that modem, using DHCP (Dynamic Host Configration Protocal).
 
 How we will get the searched file in laymans term. 
 Device Made a request, it will go to the router. From router --> Inter Service Provider --> Internet
 
