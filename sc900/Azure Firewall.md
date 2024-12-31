is a managed, cloud-based network security service that provides threat protection for your cloud workloads and resources running in Azure.

You can deploy [[Azure Firewall]] on any virtual network but the best approach is to use it on a centralized virtual network. All your other virtual and on-premises networks will then route through it. The advantage of this model is the ability to centrally exert control of network traffic for all your VNets across different subscriptions.![Diagram showing how Azure Firewall is running on a centralized virtual network can protect both cloud-based VNets and your on-premises network.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-basic-security-capabilities-azure/media/2-azure-firewall.png)
- With [[Azure Firewall]], you can scale up the usage to accomodate changing network traffic flows, so you don't need to budget for peak traffic. Network traffic is subjected to the configured firewall rules when you route it to the firewall as the subnet default gateway.
## Features
1. Stateful Firewall
	- [[Azure Firewall]] is a stateful [[firewall]], meaning it can keep track of the state of active connections & make decisions based on the context of the traffic
2. Built-in high availability & availability zones
	- [[Azure Firewall]] has built-in high [[Availability]], meaning it's designed to ensure continuous operation and minimal downtime, even in the event of failures or high traffic loads. [[Azure Firewall]] can be configured to span multiple [[Availability Zone]](s) where each availability zone is made up of one or more datacenters equipped with independent power, cooling, and networking. Azure Firewall's support for availability zones ensures higher [[availability]] and resilience by distributing resources across these separate zones.
3. Network & application level filtering
	- [[Azure Firewall]] allows you to create and enforce network traffic filtering rules for both inbound and outbound traffic. You can define rules based on IP addresses, ports, and protocols. [[Azure Firewall]] can filter traffic based on the application-layer protocols such as HTTP/S. This means you can control access to [[Fully Qualified Domain Name (FQDN)]].
4. [[Source Network Address Translation (SNAT)]] & [[Destination Network Address Translation (DNAT)]]
5. Threat intelligence
	- [[Azure Firewall]] integrates with Microsoft's Threat Intelligence feed to alert you about known malicious IP addresses and domains, helping to protect your network from threats. Threat intelligence-based filtering can be enabled for your firewall to alert and deny traffic from/to known malicious IP addresses and domains.
6. Logging & Monitoring
	- [[Azure Firewall]] provides logging & monitoring capabilities to help you keep track of [[firewall]] activity & diagnose issues. Logs can be sent to Azure Monitor, Log Analytics, or Event Hubs for further analysis
7. Integration with Azure Services
	- It integrates seamlessly with other Azure services, such as Azure Virtual Networks, Azure Policy, and Azure Security Center, providing a cohesive security solution for your cloud infrastructure.
### Integration 