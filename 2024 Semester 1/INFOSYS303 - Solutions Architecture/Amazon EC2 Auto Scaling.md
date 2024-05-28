- collection of [[Amazon EC2]] instances that are treated as a logical grouping for the purposes of [[autoscaling]] & management

1. [[Target group]]
2. [[Security group]]
- This setup allows for automated scaling & traffic management while maintaining security controls
![[Pasted image 20240528222941.png]]
[[Amazon EC2 Auto Scaling]] enables you to automatically add or remove [[Amazon EC2 instance(s)]] in response to changing application demand. By automatically scaling your instances in and out as needed, you can maintain a greater sense of application availability.

Within [[Amazon EC2 Auto Scaling]], you can use two approaches: dynamic scaling and predictive scaling.
- _Dynamic scaling_ responds to changing demand. 
- _Predictive scaling_ automatically schedules the right number of Amazon EC2 instances based on predicted demand.
## Components of AWS Auto Scaling Group
1. [[instance(s)]]
	- the group contains a collection of [[Amazon EC2 instance(s)]] that are automatically adjusted in number based on the defined conditions for scaling.
2. Scaling Options
	- it can scale out (add [[instance(s)]]) to handle increased load & scale in (remove [[instance(s)]]) when the demand stops
3. Health Checks
	- The health of [[instance(s)]] is monitored, & if any are found to be unhealthy, they are replaced to maintain the desired capacity
4. [[Load Balancing]]
	- Often integrated with [[Load Balancer(s)]] to distributed traffic evenly across the [[instance(s)]] in the group
5. High [[Availability]]
	- Spreads [[instance(s)]] across multiple [[Availability Zone]] within a region to increase fault tolerance

|                   | [[Amazon EC2 Auto Scaling]]                                                                                                                 | [[Load Balancer(s)]]                                                                                                                    |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| Purpose:          | Automatically adjust the number of [[Amazon EC2]] [[instance(s)]] in your application's architecture to handle the current load efficiently | Distributes incoming application traffic across multiple targets, such as [[Amazon EC2 instance(s)]], in multiple [[Availability Zone]] |
| Behavior:    <br> | Scales out by adding [[instance(s)]] when demand increases, & scales in by terminating [[instance(s)]] when demand decreases                | Routes user requests to [[instance(s)]] that are operational & have the capacity to serve those requests                                |
| Health:           | Monitors the health of [[instance(s)]] & replaces unhealthy ones to ensure continuous service                                               | Periodically checks the health of [[instance(s)]] & only routes traffic to the healthy ones                                             |
## How [[Amazon EC2 Auto Scaling]] & [[Load Balancer(s)]] work together
1. Dynamic Scaling
	- As traffic to your application changes, the [[Load Balancer(s)]] spreads the load across the [[instance(s)]] in the [[autoscaling]] group
2. Efficient Resource Use
	- [[autoscaling]] ensures that you have the right number of [[Amazon EC2 instance(s)]] available
	- The [[Load Balancer(s)]] then ensures that each [[instance(s)]] is used effectively
3. High [[Availability]]
	- if an [[instance(s)]] fails health checks & is deemed unhealthy by the [[Load Balancer(s)]], [[autoscaling]] can replace it without manual intervention
4. Cost Optimization
	 - By adjusting the number of [[instance(s)]] automatically, 