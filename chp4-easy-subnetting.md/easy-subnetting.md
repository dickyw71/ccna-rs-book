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
    |**Broadcast**|**63**|**128**|**191**|**255**|


