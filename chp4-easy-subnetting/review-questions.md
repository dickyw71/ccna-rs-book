# Easy subnetting - review questions

1. What is the maximum number of IP addresses that can be assigned to hosts on a local subnet that uses the 255.255.255.224 subnet mask?  
    A. 14  
    B. 15  
    C. 16  
    **D. 30 (My answer)**   
    E. 31  
    F. 62  

    .224 = 111**00000**  
    2<sup>5</sup> - 2 = 30

2. You have a network that needs 29 subnets while maximizing the number of host addresses available on each subnet. How many bits must you borrow from the host field to provide the correct subnet mask?
    A. 2  
    B. 3  
    C. 4  
    **D. 5 (My answer)**   
    E. 6  
    F. 7  

    2<sup>5</sup> = 32 subnets
    2<sup>3</sup> - 2 = 6 hosts   
    255.255.255.248
    
3. What is the subnetwork address for a host with the IP address 200.10.5.68/28?  
    A. 200.10.5.56  
    B. 200.10.5.32  
    **C. 200.10.5.64 (my answer)**  
    D. 200.10.5.0  

    Subnet mask: 255.255.255.248  
    Block size: 256 - 248 = 8  
    Subnets: .0, .8, .16, .24, .32, .40, .48, .56, .64, .72, ...  
    Subnetwork address: 200.10.5.64  

4. The network address of 172.16.0.0/19 provides how many subnets and hosts?
    A. 7 subnets, 30 hosts each  
    B. 7 subnets, 2,046 hosts each  
    C. 7 subnets, 8190 hosts each  
    D. 8 subnets, 30 hosts each  
    E. 8 subnets, 2046 hosts each  
    **F. 8 subnets, 8190 hosts each (My answer)**  
    
    Subnet mask: 255.255.224.0 
    Block size: 256 - 224 = 32  
    Subnets: 0.0, 32.0, 64.0, .96.0, .128.0, .160.0, .192.0, .224.0  
    2<sup>14</sup> - 2 = 8190 hosts in each subnet

5. Which two statements describe the IP address 10.16.3.65/23? (Choose two.)  
A. The subnet address is 10.16.3.0 255.255.255.254.0.  
**B. The lowest host address in the subnet is 10.16.2.1 255.255.254.0. (My answer)**  
C. The last valid host address in the subnet is 10.16.2.254 255.255.254.0.  
**D. The broadcast address of the subnet is 10.16.3.255 255.255.254.0. (My answer)**  
E. The network is not subnetted.  

    Class A reserved IP address  
    15 subnet bits  
    9 host bits  

    Block size: 256 - 254 = 2  
    Subnets: 2<sup>15</sup> = 32769  
    0.0, 2.0, 4.0, 6.0, 8.0, 10.0, ...  

6. If a host on a network has the address 172.16.45.14/30, what is the subnetwork this host belongs to?  
A. 172.16.45.0  
B. 172.16.45.4  
C. 172.16.45.8  
**D. 172.16.45.12 (My answer)**  
E. 172.16.45.16

    Class B reserved IP address  
    Subnet mask: 255.255.255.252  
    Block size: 256 - 252 = 4  
    45,0, 45.4, 45.8, 45.12, 45.16, 45.20, ...  

7. Which mask should you use on point-to-point WAN links on order to reduce the waste of IP addresses?  
A. /27  
B. /28  
C. /29  
**D. /30 (My answer)**  
E. /31  

8. What is the subnetwork number of a host with an IP address of 172.16.66.0/21?  
A. 172.16.36.0  
B. 172.16.48.0  
**C. 172.16.64.0 (My answer)**   
D. 172.16.0.0  

    Class B reserved IP address  
    13 subnet bits  
    11 host bits  

    Subnet mask: 255.255.248.0  
    Block size: 256 - 248 = 8  
    Subnets: 0.0, 8.0, 16.0, 32.0, 48.0, 64.0, 80.0, ...  
    Subnetwork: 172.16.64.0  

9. You have an interface on a router with an IP address of 192.168.192.10/29. Including the router interface, how many hosts can have IP addresses on the LAN attached to the router interface?  
**A. 6 (My answer)**  
B. 8  
C. 30  
D. 62  
E. 126  

    Hosts: 2<sup>3</sup> - 2 = 6  

10. You need to configure a server that is on the subnet 192.168.19.24/29. The router has the first available host address. Which of the following should you assign to the server?  
A. 192.168.19.0 255.255.255.0  
B. 192.168.19.33 255.255.255.240  
**C. 192.168.19.26 255.255.255.248 (My answer)**  
D. 192.168.19.31 255.255.255.248  
E. 192.168.19.34 255.255.255.240  

    Subnet mask: 255.255.255.248  
    Block size: 256 - 248 = 8  
    0, 8, 16, 24, 32, ...  

11. 