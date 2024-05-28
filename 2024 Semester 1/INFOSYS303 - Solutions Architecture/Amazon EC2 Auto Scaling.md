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

| [[Amazon EC2 Auto Scaling]]         |     |
| ----------------------------------- | --- |
| Purpose: Automatically adjust the n |     |
