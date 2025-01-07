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