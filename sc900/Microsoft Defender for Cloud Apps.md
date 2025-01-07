Defender for Cloud apps is a cloud access security broker that brings deep visibility, strong data controls, and enhanced threat protection to your cloud apps.

Microsoft Defender for Cloud Apps delivers full protection for [[Software as a Service (SaaS)]] applications, helping you monitor and protect your cloud app data across the following feature areas:

- Fundamental [[Cloud Access Security Broker (CASB)]] functionality. 
    
- [[SaaS Security Posture Management (SSPM)]] features, enabling security teams to improve the organization’s security posture
    
- Advanced threat protection, as part of Microsoft's extended detection and response (XDR) solution, enabling powerful correlation of signal and visibility across the full kill chain of advanced attacks
    
- App-to-app protection, extending the core threat scenarios to OAuth-enabled apps that have permissions and privileges to critical data and resources.
### Discover [[Software as a Service (SaaS)]] applications
[[Microsoft Defender for Cloud Apps]] shows the full picture of risks to your environment from [[Software as a Service (SaaS)]] app usage and resources, and gives you control of what’s being used and when.

- Identify: 
	- Defender for Cloud apps uses data based on an assessment of network traffic and an extensive app catalog to identify apps accessed by users across your organization.
    
- Assess: 
	- Evaluate discovered apps for more than 90 risk indicators, allowing you to sort through the discovered apps and assess your orgs security and compliance posture.
    
- Manage: 
	- Set policies that monitor apps around the clock. 
>		For example, if anomalous behavior happens, like unusual spikes in usage, you're automatically alerted and guided to action.
### Information protection
Defender for Cloud Apps connects to [[Software as a Service (SaaS)]] apps to scan for files containing sensitive data uncovering which data is stored where and who is accessing it. To protect this data, organizations can implement controls such as:

- Apply a sensitivity label
- Block downloads to an unmanaged device
- Remove external collaborators on confidential files

The Defender for Cloud Apps integration with [[Microsoft Purview]] also enables security teams to leverage out-of-the-box data classification types in their information protection policies and control sensitive information with data loss protection (DLP) features.
### Advanced threat protection
Cloud apps continue to be a target for adversaries trying to exfiltrate corporate data. Sophisticated attacks often cross modalities. Attacks often start from email as the most common entry point then move laterally to compromise endpoints and identities, before ultimately gaining access to in-app data.

Defender for Cloud Apps offers built-in adaptive access control (AAC), provides user and entity behavior analysis (UEBA), and helps you mitigate these types of attacks.

Defender for Cloud Apps is also integrated directly into [[Microsoft Defender XDR]], correlating eXtended detection and response (XDR) signals from the Microsoft Defender suite and providing incident-level detection, investigation, and powerful response capabilities. Integrating [[Software as a Service (SaaS)]] security into Microsoft's XDR experience gives SOC teams full kill chain visibility and improves operational efficiency and effectivity.
### App to app protection with app governance
OAuth, an open standard for token-based authentication and authorization, enables a user's account information to be used by third-party services, without exposing the user's password. Apps that use OAuth often have extensive permissions to access data in other apps on behalf of a user, making OAuth apps susceptible to a compromise.

Defender for Cloud Apps closes the gap on OAuth app security, helping you protect inter-app data exchange with application governance. With Defender for Cloud Apps, you can watch for unused apps and monitor both current and expired credentials to govern the apps used in your organization and maintain app hygiene.
### [[Microsoft Defender for Cloud Apps]] in the Microsoft Defender portal
[[Microsoft Defender for Cloud Apps]] is experienced through the Microsoft Defender portal. The Defender portal is the home for monitoring and managing security across your Microsoft identities, data, devices, apps, and infrastructure, allowing security admins to perform their security tasks, in one location.

Microsoft Defender for Cloud apps functionality can be found under the Cloud apps node on the left navigation panel of the Microsoft Defender portal. The list that follows is a subset of the functionality supported.

- Cloud discovery - Identify cloud app usage in your environment.
- Cloud app catalog - Reference information about known cloud apps.
- App governance - Get in-depth visibility and control over OAuth apps integrated with Microsoft Entra ID, Google, and Salesforce.
- Activity log - View all activities involving connected apps.
- Governance log - Review actions taken to secure cloud apps.
- Policies - Configure security policies for cloud apps.![A screenshot of the cloud discovery page in the Microsoft Defender portal.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/cloud-discovery.png)