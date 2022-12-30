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

5. 