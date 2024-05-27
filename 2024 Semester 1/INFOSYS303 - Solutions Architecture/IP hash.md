Combines incoming traffic's source & destination IP addresses & uses a mathematical function to convert it into a hash. Based on the hash, the connection is assigned to a specific server

#compsci345example ![[Pasted image 20240523002903.png]]

#compsci345example 
We have 4 servers to allocate loads across

An easy-to-understand method is to hash incoming requests (maybe by IP address or some client detail) & then generate hashes for each request.

Then we apply the modulo operator to that hash, where the right operand is the number of servers
