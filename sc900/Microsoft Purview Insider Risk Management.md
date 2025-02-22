[[Microsoft Purview]] Insider Risk Management is a solution that helps minimize internal risks by enabling an organization to detect, investigate, and act on risky and malicious activities.

Managing and minimizing risk in an organization starts with understanding the types of risks found in the modern workplace. Some risks are driven by external events and factors, and are outside an organization’s direct control. Other risks are driven by internal events and employee activities that can be eliminated and avoided. 
>Some examples include:
>- Leaks of sensitive data and data spillage
>- Confidentiality violations
>- Intellectual property (IP) theft
>- Fraud
>- Insider trading
>- Regulatory compliance violations

Insider risk management is centered around the following principles:
- **Transparency**: Balance user privacy versus organization risk with privacy-by-design architecture.
- **Configurable**: Configurable policies based on industry, geographical, and business groups.
- **Integrated**: Integrated workflow across Microsoft Purview solutions.
- **Actionable**: Provides insights to enable user notifications, data investigations, and user investigations.
## Insider risk management workflow
Insider risk management helps organizations to identify, investigate, and address internal risks. With focused policy templates, comprehensive activity signaling across Microsoft 365, and a flexible workflow, organizations can take advantage of actionable insights to help identify and resolve risky behavior quickly. Identifying and resolving internal risk activities and compliance issues with insider risk management in [[Microsoft Purview]] is achieved using the following workflow:
![A diagram of the insider risk management workflow.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/insider-risk-management-workflow.png)
- **Policies** 
	- Insider risk management policies are created using predefined templates and policy conditions that define what risk indicators are examined in Microsoft 365 feature areas. These conditions include how indicators are used for alerts, what users are included in the policy, which services are prioritized, and the monitoring time period.
    
- **Alerts** 
	- Alerts are automatically generated by risk indicators that match policy conditions and are displayed in the alerts page, which provides a quick view of all alerts needing review, open alerts over time, and alert statistics for the organization. DLP alerts can also be viewed in the [[Microsoft Defender portal]], where they are automatically combined into incidents that provide a comprehensive view into potential policy violations and advanced tools for investigation and remediation.
    
- **Triage**
	- New activities that need investigation automatically generate alerts that are assigned a _Needs review_ status. Reviewers in the organization can quickly identify these alerts and scroll through each to evaluate and triage. Alerts are resolved by opening a new case, assigning the alert to an existing case, or dismissing the alert. As part of the triage process, reviewers can view alert details for the policy match, view user activity associated with the match, see the severity of the alert, and review user profile information.
    
- **Investigate**
	- Cases are created for alerts that require deeper review and investigation of the details and circumstances around the policy match. The cases page provides an all-up view of all active cases, open cases over time, and case statistics for the organization. Selecting a case opens it for investigation and review. This area is where risk activities, policy conditions, alerts details, and user details are synthesized into an integrated view for reviewers. The primary investigation tools in this area are:
	    - User activity: 
		    - User risk activity is automatically displayed in an interactive chart that plots activities over time and by risk level for current or past risk activities. Reviewers can quickly filter and view the entire risk history for the user and drill into specific activities for more details.
	    - Content explorer: 
		    - All data files and email messages associated with alert activities are automatically captured and displayed in the Content explorer. Reviewers can filter and view files and messages by data source, file type, tags, conversation, and many more attributes.
	    - Case notes:
		    - Reviewers can provide notes for a case in the Case Notes section. This list consolidates all notes in a central view and includes reviewer and date submitted information.
- **Action**
	- After cases are investigated, reviewers can quickly act to resolve the case or collaborate with other risk stakeholders in the organization. Actions can be as simple as sending a notification when employees accidentally or inadvertently violate policy conditions. In more serious cases, reviewers may need to share the insider risk management case information with other reviewers in the organization. Escalating a case for investigation makes it possible to transfer data and management of the case to eDiscovery in [[Microsoft Purview]].

Insider risk management can help you detect, investigate, and take action to mitigate internal risks in your organization in several common scenarios. These scenarios include data theft by employees, the intentional, or unintentional leak of confidential information, offensive behavior, and more.