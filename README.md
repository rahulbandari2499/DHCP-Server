# DHCP-Server
Implemented a clone of DHCP Server in python.It follows the standard DHCP implementation sequence to allocate a IP address upon a client request in the available IP range.


## How to Start?
```
Usage: For Server use command ' ./server ' ; For Client use './client' ;

Note: Before running the above programs give permissions using ' chmod 777 server ' and ' chmod 777 client '. 
```
### Some Assumptions
```
# Server
1. server always takes in the subsconf file and it will be preprocess all the labs and does   subnetting in labs.
2. If subnetting is not possible within labs it will be output the error msg without even an client request.
3. If more clients it sends msg to client appropriately. 
4. Now we will be seeing the IP addr of server in any lab. 
5. For the remaining range we will be leaving off one address. 
# Client
1. Appropriate error msg will be printed if allocation not possible.
2. It validates the mac addresses.
3. It will check upon the flags correctly
4. It will be taking the mac address of ethernet if both are present,else single for without  flag request
```
