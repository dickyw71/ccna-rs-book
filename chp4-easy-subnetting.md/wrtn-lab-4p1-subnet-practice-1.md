# Written Lab 4.1: Subnet Practice #1

Write the subnet, broadcast address, and a valid host range for question 1 through question 6. Then answer the remaining questions.

1. 192.168.100.25/30

> This IP is in the Class C private address range 192.168.0.0 - 192.168.255.255 

|Subnet mask|Block Size|Subnets|
|-|-|-|
|255.255.255.252|4|.0, .4, .8, .12, .16, .20, .24, .28 etc.|

|Subnet|Broadcast address|Valid hosts|
|-|-|-|
|192.168.100.24|192.168.100.27|192.168.100.25 - 192.168.100.26|

2. 192.168.100.37/28

> Also a Class C private address

|Subnet mask|Block Size|Subnets|
|-|-|-|
|255.255.255.240|16|.0, .16, .32, .48, .64, .80, .96, .112 etc.|

|Subnet|Broadcast address|Valid hosts|
|-|-|-|
|192.168.100.32|192.168.100.47|192.168.100.33 - 192.168.100.46|

3. 192.168.100.66/27

> Another Class C private address

|Subnet mask|Block Size|Subnets|
|-|-|-|
|255.255.255.224|32|.0, .32, .64, .96, .128, .160, .192, .224|

|Subnet|Broadcast address|Valid hosts|
|-|-|-|
|192.168.100.64|192.168.100.95|192.168.100.65 - 192.168.100.94|

4. 192.168.100.17/29

> In Class C private address range

|Subnet mask|Block Size|Subnets|
|-|-|-|
|255.255.255.248|8|.0, .8, .16, .24, .32, .40, .48, .56 etc.|

|Subnet|Broadcast address|Valid hosts|
|-|-|-|
|192.168.100.16|192.168.100.23|192.168.100.17 - 192.168.100.22|

5. 192.168.100.99/26

> Also a Class C private address

|Subnet mask|Block Size|Subnets|
|-|-|-|
|255.255.255.192|64|.0, .64, .128, .192|

|Subnet|Broadcast address|Valid hosts|
|-|-|-|
|192.168.100.64|192.168.100.127|192.168.100.65 - 192.168.100.126|

6. 192.168.100.99/25

> A Class C private address

|Subnet mask|Block Size|Subnets|
|-|-|-|
|255.255.255.128|128|.0, .128|

|Subnet|Broadcast address|Valid hosts|
|-|-|-|
|192.168.100.0|192.168.100.127|192.168.100.1 - 192.168.100.126|

7. You have a Class B network and need 29 subnets. What is your mask?

    > Mask is 255.255.255.248

8. What is the broadcast address of 192.168.192.10/29?

    > Broadcast address 192.168.192.23

9. How many hosts are available with a Class C /29 mask?

    > 6 hosts per subnet

10. What is the subnet for host ID 10.16.3.65/23?

|Mask|Block Size|Subnets|
|-|-|-|
|255.255.254.0|2|0.0, 2.0, 4.0, 6.0, 8.0, etc.|

    > Subnet is 10.16.2.0

