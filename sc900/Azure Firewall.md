is a managed, cloud-based network security service that provides threat protection for your cloud workloads and resources running in Azure.

You can deploy [[Azure Firewall]] on any virtual network but the best approach is to use it on a centralized virtual network. All your other virtual and on-premises networks will then route through it. The advantage of this model is the ability to centrally exert control of network traffic for all your VNets across different subscriptions.![Diagram showing how Azure Firewall is running on a centralized virtual network can protect both cloud-based VNets and your on-premises network.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-basic-security-capabilities-azure/media/2-azure-firewall.png)
- With [[Azure Firewall]], you can scale up the usage to accomodate changing network traffic flows, so you don't need to budget for peak traffic. Network traffic is subjected to the configured firewall rules when you route it to the firewall as the subnet default gateway.
## Features
1. [[Stateful Firewall]]
2. [[Built-in high availability & availability zones]]
3. [[Network & application level filtering]]
4. [[Source Network Address Translation (SNAT)]] & [[Destination Network Address Translation (DNAT)]]
5. [[Threat intelligence]]