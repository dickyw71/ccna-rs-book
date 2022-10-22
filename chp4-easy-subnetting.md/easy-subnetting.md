### Class C subnet masks

|Binary octet 4|Decimal|CIDR|
|-|-|-|
|00000000|255.255.255.0|/24|
|10000000|255.255.255.128|/25|
|11000000|255.255.255.192|/26|
|11100000|255.255.255.224|/27|
|11110000|255.255.255.240|/28|
|11111000|255.255.255.248|/29|
|11111100|255.255.255.252|/30|

### Subnetting - The Five Questions

- How many subnets does the chosen subnet mask produce?  
    2<sup>*x*</sup> = number of subnets. *x* is the number of mask bits, or the 1s.  

- How many valid hosts per subnet are available?  
    2<sup>*y*</sup> - 2 = number of host per subnet. *y* is the number of unmasked bits, or the 0s.  

- What are the valid subnets?  
    256 - subnet mask = block size, or the increament number.  
    e.g. 256 - 192 = 64 block size. Count up in block size from 0  
    0, 64, 128, 192 are the valid subnets  

- What is the broadcast address of each subnet?  
    Using the example above with block size of 64   
    the broadcast addresses for each subnet are 63, 127, 191, 255  

- What are the valid hosts in each subnet?  
    Valid hosts are the numbers between subnets and broadcast addresses  
    
    |Subnet|0|64|128|192|
    |-|-|-|-|-|
    |First host|1|65|129|193|
    |Last host|62|126|190|254|
    |**Broadcast**|**63**|**127**|**191**|**255**|

### Class C Subnets

|CIDR notation|Mask|Bits|Block size|Subnets|Host|
|-|-|-|-|-|-|
|/25|128|1 bit on and 7 bits off|128|0 and 128|2 subnets, each with 126 hosts|
|/26|192|2 bits on and 6 bits off|64|0, 64, 128 and 192|4 subnets, each with 62 hosts|
|/27|224|3 bits on and 5 bits off|32|0, 32, 64, 96, 128, 160, 192 and 224| 8 subnets, each with 30 hosts|
|/28|240|4 bits on and 4 bits off|16|0, 16, 32, 48, 64, 80, 96, 112, 128, 144, 160, 176, 192, 208, 224 and 240|16 subnets, each with 14 hosts|
|/29|248|5 bits on and 3 bits off|8|0, 8, 16, 24, 32, 40, 48, etc.|32 subnets, each with 6 hosts|
|/30|252|6 bits on 2 bits off|4|0, 4, 8, 12, 16, 20, 24, etc.|64 subnets, each with 2 hosts|
