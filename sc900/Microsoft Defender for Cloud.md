[[Microsoft Defender for Cloud]] is a cloud-native application platform (CNAPP) with a set of security measures & practices designed to protect cloud-based applications from various cyber threats & vulnerabilities. Defender for Cloud combines the capabilities of:
- [[development security operations (DevSecOps)]] solution that unifies security management at the code level across multicloud & multiple-pipeline environments
- A [[cloud security posture management (CSPM)]] solution that surfaces actions that you can take to prevent breaches.
- A [[cloud workload protection platform (CWPP)]] with specific protections for servers, containers, storage, databases, and other workloads.![A s=diagram showing the three pillars fo Microsoft Defender for Cloud:  DevOps security management, cloud security posture management, and cloud workload protection platform.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-security-management-capabilities-of-azure/media/defender-for-cloud-pillars-inline.png)

Microsoft Defender for Cloud, through its [[development security operations (DevSecOps)]], [[cloud security posture management (CSPM)]], and [[cloud workload protection platform (CWPP)]] capabilities, enables organizations to manage the security of their resources and workloads in the cloud and on-premises and improve their overall security posture.

Also, for businesses that are onboarded to Microsoft Security Copilot, Microsoft Defender for Cloud embeds capabilities of Microsoft Security Copilot. Specifically, the integration with Copilot allows you to analyze, summarize, remediate, and delegate recommendations using natural language prompts.

When you enable Defender for Cloud, you automatically gain access to Microsoft Defender XDR, an enterprise defense suite that natively coordinates detection, prevention, investigation, and response across endpoints, identities, email, and applications to provide integrated protection against sophisticated attacks. 
## How Security policies & initiatives improve cloud security posture
[[Microsoft Defender for Cloud ]]enables organizations to manage the security of their resources and workloads in the cloud and on-premises and improve their overall security posture. It does this by using policy definitions and security initiatives, so it's important to understand these terms.
- An [[Azure Policy]] definition, created in [[Azure policy]]
    
- A [[security initiative]] is a collection of [[Azure Policy]] definitions, or rules, grouped together towards a specific goal or purpose. 
    
- To implement policy definitions or initiatives, you assign them to any scope of resources that are supported, such as management groups, subscriptions, resource groups, or individual resources.
    

Microsoft Defender for Cloud applies [[security initiative]] to your subscriptions. These initiatives contain one or more security policies. Each of those policies results in a security recommendation for improving your security posture.

Security administrators can build their own custom security initiatives in [[Microsoft Defender for Cloud]], but there's also a default, built-in security initiative named '[[Microsoft cloud security benchmark (MCSB)]]' that is automatically assigned when you enable [[Microsoft Defender for Cloud]] on your subscription.
## [[Microsoft cloud security benchmark (MCSB)]] in Defender for Cloud
[[Microsoft Defender for Cloud]] continuously assesses an organization's hybrid cloud environment to analyze the risk factors according to the controls and best practices in the [[Microsoft cloud security benchmark (MCSB)]]. The regulatory compliance dashboard in Microsoft Defender for Cloud reflects the status of your compliance with the MCSB and any other standards that you've applied to your subscriptions.

Some of the controls used in the MCSB include network security, identity and access control, data protection, data recovery, incident response, and more.![Screenshot of Microsoft Defender for Cloud showing status of regulatory compliance against Microsoft cloud security benchmark.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-security-management-capabilities-of-azure/media/defender-cloud-compliance-inline.png)
### Enhanced security of [[Microsoft Defender for Cloud]]
A pillar of cloud security is cloud workload protection. Through cloud workload protection capabilities, [[Microsoft Defender for Cloud]] is able to detect and resolve threats to resources, workloads, and services. Cloud workload protections are delivered through integrated Microsoft Defender plans, specific to the types of resources in your subscriptions and provide enhanced security features for your workloads.

#### Defender plans
[[Microsoft Defender for Cloud]] includes a range of advanced intelligent protections for your workloads. The workload protections are provided through Microsoft Defender plans specific to the types of resources in your subscriptions. Some of the Microsoft Defender for Cloud plans you can select from include:

- **Microsoft Defender for servers** adds threat detection and advanced defenses for your Windows and Linux machines.
- **Microsoft Defender for App Service** identifies attacks targeting applications running over App Service.
- **Microsoft Defender for Storage** detects potentially harmful activity on your Azure Storage accounts.
- **Microsoft Defender for SQL** secures your databases and their data wherever they're located.
- **Microsoft Defender for Kubernetes** provides cloud-native Kubernetes security environment hardening, workload protection, and run-time protection.
- **Microsoft Defender for container registries** protects all the Azure Resource Manager based registries in your subscription.
- **Microsoft Defender for Key Vault** is advanced threat protection for Azure Key Vault.
- **Microsoft Defender for Resource Manager** automatically monitors the resource management operations in your organization.
- **Microsoft Defender for DNS** provides an additional layer of protection for resources that use Azure DNS's Azure-provided name resolution capability.
- **Microsoft Defender for open-source relational protections** brings threat protections for open-source relational databases.
These different plans can be enabled separately and will run simultaneously to provide a comprehensive defense for compute, data, and service layers in your environment.
#### Enhanced security features
Microsoft Defender plans specific to the types of resources in your subscriptions provide enhanced security features for your workloads. Listed below are some of the enhanced security features.

- Comprehensive endpoint detection and response - Microsoft Defender for servers includes Microsoft Defender for Endpoint for comprehensive endpoint detection and response (EDR).
    
- Vulnerability scanning for virtual machines, container registries, and SQL resources - Easily deploy a scanner to all of your virtual machines. View, investigate, and remediate the findings directly within Microsoft Defender for Cloud.
    
- Multicloud security - Connect your accounts from Amazon Web Services (AWS) and Google Cloud Platform (GCP) to protect resources and workloads on those platforms with a range of Microsoft Defender for Cloud security features.
    
- Hybrid security – Get a unified view of security across all of your on-premises and cloud workloads. Apply security policies and continuously assess the security of your hybrid cloud workloads to ensure compliance with security standards. Collect, search, and analyze security data from multiple sources, including firewalls and other partner solutions.
    
- Threat protection alerts - Monitor networks, machines, and cloud services for incoming attacks and post-breach activity. Streamline investigation with interactive tools and contextual threat intelligence.
    
- Track compliance with a range of standards - Microsoft Defender for Cloud continuously assesses your hybrid cloud environment to analyze the risk factors according to the controls and best practices in Azure Security Benchmark. When you enable the enhanced security features, you can apply a range of other industry standards, regulatory standards, and benchmarks according to your organization's needs. Add standards and track your compliance with them from the regulatory compliance dashboard.
    
- Access and application controls - Block malware and other unwanted applications by applying machine learning powered recommendations adapted to your specific workloads to create allowlists and blocklists. Reduce the network attack surface with just-in-time, controlled access to management ports on Azure VMs. Access and application controls drastically reduce exposure to brute force and other network attacks.
    

Additional benefits include threat protection for the resources connected to the Azure environment and container security features, among others. Some features may be associated with specific Defender plans for specific workloads.![Screenshot showing feature set of Microsoft Defender for Cloud. The feature set without enhanced security consists of continuous assessments and secure score.  The enhanced security features that are part of Defender plans adds just-in-time access, threat protection, adaptive controls and more.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-security-management-capabilities-of-azure/media/defender-for-cloud-enhanced-features-inline.png)