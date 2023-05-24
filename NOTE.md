### Let’s subnet your home network // You SUCK at subnetting // EP 6

EP 5 

Wireless

IOT

DMZ

user 

Subnet : 192.168.1.0 /24
/24 : 11111111.11111111.11111111.00000000
255.255.255.0 (Subnet Mask)

Calculating numberd of bits needed to create 4 networks ( Based on Binary x2) \
Binary Tab : 128 - 64 - 32 - 16 - 8 - 4 - 2 - 1 ----> Ref scale \
Binary (x2): 256 -128 -64 - 32 -16 -8 - 4 - 2 ---> Number of network needed \
So we need two bits for 4 networks. \
To make 17 networks, we would need to start at 32, so fives bits on the ref scale. 

So, for 4 subnetwork: \
26/ : 11111111.11111111.11111111.11000000 \
Last bit is the increment. \
Based on binary Tab, 64 would be the increment. \
Subnet : 255.255.255.192 /26 

Network 1 : \
192.168.1.0-192.168.1.63 \
Network 2 : \
192.168.1.64-192.168.1.127 \
Network 3 : \
192.168.1.128-192.168.1.191 \
Network 4 : \
192.168.1.192-192.168.1.255

How many host ? \
6 bit access (2 a la 6), sur Binary x2, that would be 64 each network, less the network and broadcast adress, so 62 each.

