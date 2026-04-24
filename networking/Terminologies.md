## switches : stores information (mac addresses)

* used to connect different devices with each other

* can be of different sizes : 8 port , 48 port ,etc

* hub : repeat that electrical singnal (message) to every connected device

* switch identify the end device with the help of CAM(content addressable Memory) table , which have Fastethernet 0/1/2... Fa0/1, Fa0/2, etc (port) and MAC(media access control) address of the end device (unique address of a device)

* a switch is a layer 2 device , layer 3 is not involved in a switch

* cli command for switch : show mac-address-table

### layer 1 : electrical cable   , layer 2 : mac address , layer 3 : IP address

## Routers : job is to connect different networks

* layer 3 is also involved in routing

* gateway is needed to connect between networks (in networking gateway is another term for router )

* Different group of IP addresses ie. network1 = ip : 192.168.1.1 and network2 = ip : 192.168.2.1 , subnet mask can be same or different

* you first connect each network to a separate router interface using appropriate cables. Then, each interface of the router must be configured with an IP address that belongs to the respective network, and the interfaces must be activated using the no shutdown command.

* After configuring the router, all devices (PCs) in each network must be assigned IP addresses within their network range and, most importantly, a default gateway, which is the IP address of the router interface connected to their network. The router then receives data packets from one network, examines the destination IP address, and forwards the packets to the appropriate network through the correct interface.

##  `Birth of INTERNET` 

* ARPANET : Department of Defence (U.S) in 1969

* Inernet Models are designed for standardisation of networking design (Apple computer can communicate with windows computers)

### 1. TCP/IP model (4 layers) :  

* physical layer : layer1.1 (optical cables,etc)
  
* data link layer : layer1.2 (mac addresses)

* network layer : layer2 (IP addresses)
 
* transport layer : layer3 (TCP/UDP communication , Reliable data transfer)

* application layer : layer4 (All user-level protocols (HTTP, DNS, etc))

### 2. OSI model (7 layers) :  

* physical layer : layer1 (optical cables,etc)
  
* data link layer : layer2 (mac addresses)

* network layer : layer3 (IP addresses)
 
* transport layer : layer4 (Reliable data transfer TCP)

* * session layer : layer5 (Manages sessions between devices)

* * presentation layer : layer6 (Data format, encryption, compression)

* application layer : layer7 (User interaction (HTTP, FTP, DNS))

  
