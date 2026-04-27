### Some WELL KNOWN ports : 

* 21 : FTP : File Transfer Protocol 

* 22 :  SSH : Secure SHell

* 23 : Telnet

* 25 : SMTP : simple mail transfer protocol

* 80 : HTTP : HyperText transfer Protocol

* 115 : SFTP : Simple File transfer protocol

* 123 : NTP : Network Time Protocol
  
* 443 : HTTPS : HyperText Transfer Protocol Secure

* UDP port 69 : TFTP : Trivial File Transfer Protocol

## BAD networks : 

* never have a "single point of failure" , if one breaks all disrupts

* don't connect multiple switches, router->switch1->switch2->switch3 ; like a series connection
  
## GOOD networks :

### 2-Tier Architecture :

* use parallel connection : router1->switch1, router1->switch2, router1->switch3 (but not an ideal option for End-Devices communication)

* best option is to use a multilayer switch (layer3) just after a router :

* `Tier 2 called Distribution Layer` : It simply distributes the network (router and multilayer switch)  router -> multilayer_switch 

* `Tier 1 called Access Layer` : components access the network (switches and End devices) multilayer_switch->switch1, multilayer_Switch->switch2, multilayer_Switch->switch3

*  final network : router1-> multilayer_switch1 & multilayer_switch2 and router2-> multilayer_switch1 & multilayer_switch2 

*  multilayer_switch1  <->  multilayer_switch2

* multilayer_switch1 -> switch1 , switch2, switch3 and multilayer_switch2 -> switch1 , switch2, switch3

* switch1 -> PC1,PC2 and switch2 -> PC3 , server1 and switch3 -> server2, server3

### 3-Tier Architecture : 

* bottom 2 layers (distribution and access ) are exactly same as above final network

* 1 more layer `Tier 3 called Core Layer` : FASTEST SWITCHING PATHS IN NETWORKS , Its the core switch Layer between router and distribution switches, manages alot traffic

* final network : exactlty same as Tier2 : difference is 2 core switches between routers and distribution switches

## Data Centre Networks : 

* A data centre is a specialized facility used to store, manage, and process large amounts of digital data using servers, networking equipment, and storage systems.

* North/South Network : Intenet <-> servers , East/West Network : Servers <-> Servers

### `Spine - Leaf Design` of Data centre, specifically for East/West Network

* ** predictable and reliable : 2 hops between any two east/west server

* leaf Switches(access switches) and spine switches (distribution switches)

* Each leaf switch is connected with every spine switch for faster network (connection between these switches is layer3 ie IP addresses are involved)

* ALSO, Every leaf switch is connected with each spine switch

* PE : Provider Edge router and CE : Customer Edge Router
