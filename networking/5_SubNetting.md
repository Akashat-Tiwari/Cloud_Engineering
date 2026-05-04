### Subnetting : Subnetting is the process of dividing a large network into smaller networks (subnets).

* 255.255.255.0 = 11111111.11111111.11111111.00000000 (1 for network bit and 0 for host bit)

* numbers(bits) are contiguous 

* no. of host devices = 2^(no. of 0's)  - 2 (starting IP as network address and last IP as broadcast address)

* no. of host devices = 2^8 -2 = 254 host devices possible

*  changing the subnet mask as per our requirements ie subnetting : 11111111.11111111.11111110.00000000

    * now no. of hosts are = 2^9 -2 = 510 and subnet mask is changed to 255.255.254.0  
