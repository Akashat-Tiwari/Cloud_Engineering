## IP Addresses : 

* IP Address : An IP (Internet Protocol) Address is a unique numerical identifier assigned to each device on a network, used to identify and communicate with other devices.

* Subnet Mask : A Subnet Mask is a numerical value used to divide an IP address into network and host portions, helping determine whether a device is on the same network or a different one.

* Default Gateway :A Default Gateway is the network device (usually a router) that forwards data packets from a local network to other networks, such as the internet.

* Term	   |Meaning	   |Example    	|Analogy
  
* IP Address	   |Device identity	    |192.168.1.10	   |Home address

* Subnet Mask     	|Network vs host	     |255.255.255.0	    |Area/colony boundary

* Default Gateway    	|Exit point/router	      |192.168.1.1	      |Main gate

### How many IP's

* for -> Ip : 192.168.1._ and subnet mask : 255.255.255.0 : 256(x) and 253(correct) as starting, ending and default gateway IP's are reserved (192.168.1.0,192.168.1.255 and 192.168.1.1) as network address, Broadcast address and dafault gateway

### Ran out of IP Addresses : 

* there are 2^32 IP adresses that is 4,294,967,296 ie around 4 billion IP's

`classified into 5 classes (A,B,C,D and E)` 

* What are IP Classes? : IP classes are a way to divide IP addresses into groups based on network size and usage.

* Class A
  Range: 1.0.0.0 – 126.255.255.255
  Subnet Mask: 255.0.0.0
  Use: Very large networks

   *  First part = network, rest = devices
   *  Supports around 16 million of devices

* Class B
  Range: 128.0.0.0 – 191.255.255.255
  Subnet Mask: 255.255.0.0
  Use: Medium-sized networks

   *  First two parts = network
   *  Supports thousands of devices
 
* Class C
  Range: 192.0.0.0 – 223.255.255.255
  Subnet Mask: 255.255.255.0
  Use: Small networks (most common in homes/offices)

   * First three parts = network
   * Supports up to 254 devices
 
*  Class D
   Range: 224.0.0.0 – 239.255.255.255
   Use: Multicasting (sending data to multiple devices at once)
 
    *   Not used for normal device addressing
  
* Class E
  Range: 240.0.0.0 – 255.255.255.255
  Use: Experimental / research

  * Not used in general networking
 
 * Range: 127.0.0.0 – 127.255.255.255 : It is reserved for loopback (localhost), Used by a computer to communicate with itself, commonly used 127.0.0.1 
