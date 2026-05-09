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

### DHCP (Dynamic Host Configuration Protocol) : 

* Its purpose is to automatically assign IP addresses and network settings to devices on a network.

* Why DHCP is Needed

   * Every device on a network needs:
   * IP address
   * Subnet mask
   * Default gateway
   * DNS server
   * Without DHCP, you would have to configure all these manually for every device.
   * DHCP automates this process
   * Router’s DHCP server automate this process 

### DNS (Domain Name System): 

* Its a protocol and its main purpose is to translate human-readable website names (Domain names) into IP addresses that computers use to communicate.

### Simple Working Process

* When you enter a website in the browser:

    * Browser checks if it already knows the IP (cache).
    * If not, it asks a DNS server. (data center that stores domain names to its correspomding IP address)
    * DNS server finds the corresponding IP address.
    * Browser connects to that IP.
    * Website opens.
 
* nslookup command (name server lookup) : used to get the IP of the specified domain name (PC should be connected with a DNS server, like dns.google ie 8.8.8.8)

   * nsloolup youtube.com -> using dns.google (8.8.8.8)
   * output >> Name : youtube.com,
               IPV4 : 172.217.25.110,
               IPV6 : 2024:6800:4004:819:200e

* DNS cache : A DNS cache is temporary storage that keeps/saves recently visited domain name and IP address mappings. It helps devices access websites faster without asking the DNS server every time.

### DNS configuration : 

* configuring a router to be a DNS server :

   * Configuring a router as a DNS server means the router will handle DNS requests from devices in the network instead of each device directly contacting external DNS servers.
   * Without router DNS handling: Laptop → Google DNS (8.8.8.8)
   * With Router as DNS Server : Laptop → Router → External DNS Server

* configuring a router to be a DNS client :

    * Configuring a router as a DNS client means the router itself uses another DNS server to resolve domain names requests.
    * Router → External DNS Server
    * The router sends DNS queries to upstream/external DNS servers like:
          * Google DNS
          * Cloudflare DNS
          * ISP DNS servers

* 'A' records map hostnames to IPV4 addresses and 'AAAA' records hostnames to IPV6 addresses

* Ques : PC1 is configured to use an external server 8.8.8.8 as its DNS server . what DNS command is necessary on R1 to enable this?
    * Ans : No DNS configurations are needed on R1 , (but we can do if we want).
 
        ` dns.google.com --- INTERNET --- Router(R1) --- Switch --- PC1, PC2 and PC3 `
 


  
