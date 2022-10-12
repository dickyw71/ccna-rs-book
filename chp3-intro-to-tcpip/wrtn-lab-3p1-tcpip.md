# Written Lab 3.1: TCP/IP

1. What is the Class C address range in decimal and in binary?

    |Format|1st Octet Min|1st Octet Max|
    |-|-|-|
    |Decimal|192|223|
    |Binary|**110**00000|**110**11111|

    Class C range range 192.0.0.1 - 223.255.255.254
---

2. What layer of the DoD model is equivalent to the Transport layer of the OSI model?

    The DoD model **Host-to-Host** layer is equivalent to the OSI model Transport layer.  
---   

3. What is the valid range of a Class A network address?

    1.0.0.1 - 126.255.255.254
---

4. What is the 127.0.0.1 address used for?

    *localhost* local loop-back address
---

5. How do you find the network address from a listed IP address?

    From the Listed IP address:  172.16.32.64  
    - First match the IP address to the address Class  
        172.16.32.64 is a Class B address in the range 128.0.0.1 - 191.255.255.254  
    - A Class B address has the first 2 bytes for the network and the second 2 bytes for the hosts.

        >    *network.network.host.host*  

    - The network address is 172.16.0.0
---

6. How do you find the broadcast address from a listed IP address?

    From the Listed IP address:  172.16.32.64  
    - First match the IP address to the address Class  
        172.16.32.64 is a Class B address in the range 128.0.0.1 - 191.255.255.254  
    - A Class B address has the first 2 bytes for the network and the second 2 bytes for the hosts.

        >    *network.network.host.host*  

    - The broadcast address is 172.16.255.255
---

7. What is the Class A private IP address space?

    > Class A = **10.0.0.0 - 10.255.255.255**
---

8. What is the Class B private IP address space?

    > Class B = **172.16.0.0 - 172.31.255.255**
---

9. What is the Class C private Ip address space?

    > Class C = **192.168.0.0 - 192.168.0.0**
---

10. What are all the available characters that you can use in hexadecimal addressing?

    > 0 1 2 3 4 5 6 7 8 A B C D E F
---


