## Subnetting :

* Subnetting is the process of dividing a large network into smaller networks (subnets).

* 255.255.255.0 = 11111111.11111111.11111111.00000000 (1 for network bit and 0 for host bit)

* numbers(bits) are contiguous 

* no. of host devices = 2^(no. of 0's)  - 2 (starting IP as network address and last IP as broadcast address)

* no. of host devices = 2^8 -2 = 254 host devices possible

*  changing the subnet mask as per our requirements ie subnetting : 11111111.11111111.11111110.00000000

    * now no. of hosts are = 2^9 -2 = 510 and subnet mask is changed to 255.255.254.0
 
### Load Balancer : 

* A load balancer is a system that distributes incoming network traffic across multiple servers to ensure that no single server becomes overloaded, thereby improving performance, reliability, and availability of applications.

* It acts as an intermediary between users and servers, receiving client requests and intelligently forwarding them to the most suitable server based on factors like current load or availability.

* Load balancers can be implemented as hardware devices or software solutions and are widely used in modern web applications to achieve scalability and fault tolerance.

### Firewalls : 

* A firewall is a network security system that monitors and controls incoming and outgoing traffic.
 
* It acts as a barrier between a trusted network and untrusted networks (like the internet).

* Its main function is to allow or block data packets based on security rules.

* Firewalls check data using:
  
    * IP address
    * Port number
    * Protocol
 
* Common types include packet-filtering firewalls, stateful inspection firewalls, proxy firewalls, and next-generation firewalls that provide advanced features like intrusion detection and application-level filtering

* Firewalls help protect systems from cyber threats such as hacking, malware, and unauthorized access, and are an essential component of network security.
