let you filter network traffic to and from Azure resources in an Azure virtual network; for example, a virtual machine. 

A [[Network Security Groups (NSGs)]] consists of rules that define how the traffic is filtered. You can associate only one network security group to each [[virtual network]] [[subnet(s)]] and network interface in a virtual machine. The same [[Network Security Groups (NSGs)]], however, can be associated to as many different [[subnet(s)]] and network interfaces as you choose.

In the highly simplified diagram that follows, you can see an Azure [[virtual network]] with two [[subnet(s)]] that are connected to the internet, and each subnet has a virtual machine. Subnet 1 has an [[Network Security Groups (NSGs)]] assigned to it that's filtering inbound and outbound access to VM1, which needs a higher level of access. In contrast, VM2 could represent a public-facing machine that doesn't require an [[Network Security Groups (NSGs)]].![Diagram showing a simplified virtual network with two subnets each with a dedicated virtual machine resource, the first subnet has a network security group and the second subnet doesn't.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-basic-security-capabilities-azure/media/2-virtual-network.png)
### Inbound & outbound security rules
A [[Network Security Groups (NSGs)]] is made up of inbound and outbound security rules. [[Network Security Groups (NSGs)]] security rules are evaluated by priority using five information points: 
1. source
2. source port
3. destination
4. destination port
5. protocol 
- to either allow or deny the traffic. 
By default, Azure creates a series of rules, three inbound and three outbound rules, to provide a baseline level of security. You can't remove the default rules, but you can override them by creating new rules with higher priorities.

Each rule specifies one or more of the following properties:
1. **Name**: Every NSG rule needs to have a unique name that describes its purpose. For example, AdminAccessOnlyFilter.
2. **Priority**: Rules are processed in priority order, with lower numbers processed before higher numbers. When traffic matches a rule, processing stops. This means that any other rules with a lower priority (higher numbers) won't be processed.
3. **Source or destination**: Specify either individual IP address or an IP address range, service tag (a group of IP address prefixes from a given Azure service), or application security group. Specifying a range, a service tag, or application security group, enables you to create fewer security rules.
4. **Protocol**: What network protocol will the rule check? The protocol can be any of: TCP, UDP, ICMP or Any.
5. **Direction**: Whether the rule should be applied to inbound or outbound traffic.
6. **Port range**: You can specify an individual or range of ports. Specifying ranges enables you to be more efficient when creating security rules.
7. **Action**: Finally, you need to decide what will happen when this rule is triggered.

The screenshot that follows shows the default inbound rules and outbound, which are included in all NSGs.