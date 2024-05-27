acts as the "traffic cop" sitting in front of your servers & routing client requests across all servers capable of fulfilling those requests

It maximizes speed & capacity utilization & ensures that no one server is overworked, which could degrade performance

If a single server goes down, the [[Load Balancer]] redirects traffic the remaining online servers. (rebalancing)

When a new server is added to the server group, the [[Load Balancer]] automatically starts to send requests to it.
## Functions
- Distributes client requests or network load efficiently across multiple servers
- Ensures high availability & reliability by sending requests only to servers that are online
- Provides the flexibility to add/subtract servers as demand dictates
## How does the [[Load Balancer]] decide on which server to use?
#### 1. Static [[Load Balancing]] Algorithms
- [[Round robin]]
- [[Weighted round robin]]
- [[IP hash]]
	Generally use different algorithms to move traffic around

#### 2. Dynamic [[Load Balancing]] Algorithms
server is informing the [[Load Balancer]] with the state
- [[Least connection]]
- [[Weighted Least Connection]]
- [[Weighted response time]]
