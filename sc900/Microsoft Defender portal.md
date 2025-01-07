A unified security operations platform is a fully integrated toolset for security teams to prevent, detect, investigate, and respond to threats across their entire environment. For Microsoft, this means delivering the best of [[Security Information and Event Management (SIEM)]], XDR, posture management, and threat intelligence with advanced generative AI as a single platform.

Through the [[Microsoft Defender portal]], Microsoft delivers on the promise of a unified security operations platform so you can view the security health of your organization. The [[Microsoft Defender portal]] combines protection, detection, investigation, and response to threats across your entire organization and all its components, in a central place.

To access the portal, You must be assigned an appropriate role, such as Global Administrator, Security Administrator, Security Operator, or Security Reader in [[Microsoft Entra ID]] to access the [[Microsoft Defender portal]].

The Defender portal emphasizes quick access to information, simpler layouts, and bringing related information together for easier use.![A screenshot of the Microsoft Defender portal home page.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/defender-portal.png)
The [[Microsoft Defender portal]] home page shows many of the common cards that security teams need. The composition of cards and data depends on the user role. Because the Microsoft Defender portal uses role-based access control, different roles see cards that are more meaningful to their day-to-day jobs.

The [[Microsoft Defender portal]] allows you to tailor the navigation pane to meet daily operational needs. You can customize the navigation pane to show or hide functions and services based on their specific preferences. Customization is specific to you, so other admins won’t see these changes.

The left navigation pane provides easy access to the suite of [[Microsoft Defender XDR]] services. You also get access to [[Microsoft Sentinel]] and many other capabilities The sections that follow provide a brief description of the capabilities accessible from the left navigation bar in the [[Microsoft Defender portal]].
# Exposure management
Microsoft Security Exposure Management is a security solution that provides a unified view of security posture across company assets and workloads. Security Exposure Management enriches asset information with security context that helps you to proactively manage attack surfaces, protect critical assets, and explore and mitigate exposure risk.

With Security Exposure Management you can discover and monitor assets, get rich security insights, investigate specific risk areas with security initiatives, and track metrics across the organization to improve security posture.![A screenshot of the Exposure Management overview in the Microsoft Defender portal.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/exposure-management.png)
### Attack surface
![A screenshot of an attack path under Exposure Management.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/attack-path.png)
Security Exposure Management automatically generates attack paths based on the data collected across assets and workloads. It simulates attack scenarios, and identifies vulnerabilities and weaknesses that an attacker could exploit.
### Security Insights
![A screenshot of the initiatives page in Exposure Management.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/initiatives.png)
Security Exposure Management automatically generates attack paths based on the data collected across assets and workloads. It simulates attack scenarios, and identifies vulnerabilities and weaknesses that an attacker could exploit.
### Secure score
![A screenshot of the secure score page in Exposure Management.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/secure-score.png)
Microsoft Secure Score, one of the tools in the Microsoft Defender portal, is a representation of a company's security posture. The higher the score, the better your protection. From a centralized dashboard in the Microsoft Defender portal, organizations can monitor and work on the security of their Microsoft 365 identities, apps, and devices.

Secure Score provides a breakdown of the score, the improvement actions that can boost the organization's score, and how well the organization's Secure Score compares to other similar organizations.
### Data connectors
![A screenshot of the data-connectors page in Exposure Management.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/data-connectors.png)
Using data connectors you can connect data sources for a richer, more centralized exposure management experience.
# Investigation & response
![A screenshot of the Microsoft Defender portal showing the selections available for investigation and response. They are incidents and alerts, hunting, actions and submissions, and partner catalog.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/investigation-response-v2.png)
The investigation and response tab includes access to incidents and alerts, hunting, actions & submissions, and a partner catalog.
### Incidents & alerts
![A screenshot of the Microsoft Defender portal incidents page.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/incidents.png)
![A screenshot of the incident details page for a selected incident in the Microsoft Defender portal.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/incident-details.png)
An incident in the [[Microsoft Defender portal]] is a collection of related alerts, assets, investigations, and evidence to give you a comprehensive look into the entire breadth of an attack. It serves as a case file that your SOC can use to investigate that attack and manage, implement, and document the response to it. Because the [[Microsoft Defender portal]] is built upon a unified security operations platform, you get a view of all incidents including incidents generated from the suite of [[Microsoft Defender XDR]] solutions, [[Microsoft Sentinel]], and other solutions.

Within an incident, you analyze the alerts that affect your network, understand what they mean, and collate the evidence so that you can devise an effective remediation plan. The information provided for an incident includes:
- The full story of the attack, including all the alerts, assets, and remediation actions taken.
- All the alerts related to the incident.
- All the assets (devices, users, mailboxes, and apps) that have been identified to be part of or related to the incident.
- All the automated investigations triggered by the alerts in the incident.
- All the supported evidence and response.

If your organization is onboarded to [[Microsoft Security Copilot]] you can also view an incident summary, guided responses, and more.
### Hunting
![A screenshot of the advanced hunting page in the Microsoft Defender portal.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/hunting.png)
Advanced hunting is a query-based threat hunting tool that lets you explore up to 30 days of raw data, from [[Microsoft Defender XDR]] and [[Microsoft Sentinel]]. You can proactively inspect events in your network to locate threat indicators and entities, through hunting queries. Hunting queries can be created via the query editor, if you're familiar with Kusto Query Language (KQL), using a query builder, or through [[Microsoft Security Copilot]]. For users onboarded to [[Microsoft Security Copilot]], you can make a request or ask a question in natural language and Security Copilot generates a KQL query that corresponds to the request.

You can use the same threat hunting queries to build custom detection rules. These rules run automatically to check for and then respond to suspected breach activity, misconfigured machines, and other findings.
### Actions & submissions
The unified Action center brings together remediation actions across [[Microsoft Defender for Endpoint]] and [[Microsoft Defender for Office 365]]. It lists pending and completed remediation actions for your devices, email & collaboration content, and identities in one location.

In Microsoft 365 organizations with Exchange Online mailboxes, admins can use the Submissions page in the [[Microsoft Defender portal]] to submit messages, URLs, and attachments to Microsoft for analysis.
### Partner catalog
The partner catalog lists supported technology partners and professional services that can help your organization enhance the detection, investigation, and threat intelligence capabilities of the platform.
# Threat intelligence
![A screenshot of the device inventory page in the Microsoft Defender portal.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/assets-devices.png)
### Assets
