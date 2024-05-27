Combines incoming traffic's source & destination IP addresses & uses a mathematical function to convert it into a hash. Based on the hash, the connection is assigned to a specific server

#compsci345example ![[Pasted image 20240523002903.png]]

#compsci345example 
We have 4 servers to allocate loads across

An easy-to-understand method is to hash incoming requests (maybe by IP address or some client detail) & then generate hashes for each request.

Then we apply the modulo operator to that hash, where the right operand is the number of servers.![[Pasted image 20240527231831.png]]

The [[Load Balancer]] can be configured to [[IP hash]] the IP address of incoming requests & use the hash value to determine which server to redirect the request to.![[Pasted image 20240527232020.png]]

- Hashing $\rightarrow$ can cause collisions where 2 numbers hashed may be the same
## [[IP hash]] methods
1. URL hash method
2. Domain hash method
3. Destination IP hash method
4. Source IP hash method
5. De