# Written Lab 5

For each of the following sets of networks, determine the summary address and the mask to be used that will summarize the subnets.

1. 192.168.1.0/24 through 192.168.12.0/24

First host address  
192.168.1.1  
Last host address  
192.168.12.254  

Each /24 subnet has a block size is 256  
For 12 /24 subnets can use a block size of 4, 8 or 16, 32,  in octet 3
- Option with block size 4  
    - Subnets 0, 4, 8, 12, 16, ... 252  
    - 64 subnets from 192.168.1.0/24 up to 192.168.252.0/24  
    - Summary address: 192.168.1.0/23   
    - Mask: 255.255.252.0  
    - Host address range 1: 192.168.1.1 - 192.168.4.254
    - Host address range 2: 192.168.5.1 - 192.168.8.254
    - Host address range 3: 192.168.9.1 - 192.168.12.254
Summarized subnet has plenty of room for growth but may not want to have all those subnets in the summary route.  
- Option with block size 8  
    - Subnets 0, 8, 16, 24, ... 248
    - 32 subnets from 192.168.1.0 up to 192.168.248.0
    - Summary address: 192.168.1.0/22
    - Mask: 255.255.248.0
    - Host range 1: 192.168.1.1 - 192.168.8.254
    - Host range 2: 192.168.9.1 - 192.168.12.254
Summarized subnet has plenty of room for growth but may not want to have all those subnets in the summary route. 

- Option with block size 16
    - Subnets 0, 16, 32 ... 240
    - 16 subnets from 192.168.1.0
    - **Summary address: 192.168.1.0/20** 
    - **Mask: 255.255.240.0**
    - Host range: 192.168.1.1 - 192.168.15.254


2.  172.144.0.0 through 172.159.0.0

    /16

    128 + 16 = 144 + 16 = 160

    256 - 240 = 16

    128 + 64 + 32 + 16 = 240

    Summary address: 172.144.0.0/12  
    255.240.0.0

3. 192.168.32.0 through 192.168.63.0

    32  
    256 - 224 = 32  

    Summary address: 192.168.32.0/19  
    Mask: 255.255.224.0  

4. 192.168.96.0 through 192.168.111.0

    0, 16, 32, 48, 64, 80, 96, 112  
    256 - 240 = 16

    Summary address: 192.168.96.0/20  
    Mask: 255.255.240.0

5. 66.66.0.0 through 66.66.15.0

    Summary address: 66.66.0.0/20  
    Mask: 255.255.240.0

6. 192.168.1.0 through 192.168.120.0

    256 - 128 = 128  
    
    Summary address: 192.168.0.0/17  
    Mask: 255.255.128.0

7. 172.16.1.0 through 172.16.7.0

    256 - 248 = 8  

    Summary address: 172.16.0.0/21  
    Mask: 255.255.248.0

8. 192.168.128.0 through 192.168.190.0

    256 - 192 = 64  

    Summary address: 192.168.128.0/18  
    Mask: 255.255.192.0

9. 53.60.96.0 through 53.60.127.0

    256 - 224 = 32  
    128 + 64 + 32 = 224  

    Summary address: 53.60.96.0/19  
    Mask: 255.255.224.0

10. 172.16.10.0 through 172.16.63.0

    256 - 192 = 64  

    Summary address: 172.16.0.0/18  
    Mask: 255.255.192.0