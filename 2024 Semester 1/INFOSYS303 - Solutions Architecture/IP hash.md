Combines incoming traffic's source & destination IP addresses & uses a mathematical function to convert it into a hash. Based on the hash, the connection is assigned to a specific server

#compsci345example ![[Pasted image 20240523002903.png]]

#compsci345example 
We have 4 servers to allocate loads across

An easy-to-understand method is to hash incoming requests (maybe by IP address or some client detail) & then generate hashes for each request.

Then we apply the modulo operator to that hash, where the right operand is the number of servers.![[Pasted image 20240527231831.png]]

The [[Load Balancer]] can be configured to [[IP hash]] the IP address of incoming requests & use the hash value to determine which server to redirect the request to.![[Pasted image 20240527232020.png]]

- Hashing $\rightarrow$ can cause collisions where 2 numbers hashed may be the same
- Hashes are shorter & easier to use than the information that they are based on, while retaining enough information to ensure that no 2 different pieces of information generate the same hash & are therefore confused with 1 another
- You can the hashing [[Load Balancing]] methods in an environment where a cache serves a wider range of content from the Internet or specified origin servers
- Caching requests $\rightarrow$ reduces request & response latency & ensures better resource (CPU) utilization, making caching popular on heavily used websites & application servers
- Since these sites also benefit from [[Load Balancing]], hashing [[Load Balancing]] methods are widely useful
## [[IP hash]] methods
1. URL hash method
2. Domain hash method
3. Destination IP hash method
4. Source IP hash method
5. Source Destination IP hash method
6. Source IP Source Port hash method
7. Call ID hash method
8. Token method