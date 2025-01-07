Threat intelligence analysts struggle with balancing a breadth of threat intelligence ingestion with the analysis of which threat intelligence poses the biggest threats to their organization and/or industry. Similarly, vulnerability intelligence analysts battle correlating their asset inventory with Common Vulnerabilities and Exposures (CVE) information to prioritize the investigation and remediation of the most critical vulnerabilities associated with their organization.

[[Microsoft Defender Threat Intelligence (Defender TI)]] addresses these challenges by aggregating and enriching critical data sources and displaying them in an innovative, easy-to-use interface. Analysts can then correlate indicators of compromise (IOCs) with related articles, actor profiles, and vulnerabilities. Defender TI also lets analysts collaborate with fellow Defender TI-licensed users within their tenant on investigations.

Microsoft Defender Threat Intelligence functionality includes:
- [[Threat analytics]]
- [[Intel Profiles]]
- [[Intel Explorer]]
- [[Intel Projects]]
### [[Microsoft Defender Threat Intelligence (Defender TI)]] in the Microsoft Defender portal
Microsoft Defender TI is experienced through the Microsoft Defender portal.

The Threat intelligence node on the navigation panel of the Microsoft Defender portal is where you can find the Microsoft Defender Threat Intelligence functionality.
![A screenshot of the selectable options for threat intelligence on the left navigation panel of the Microsoft Defender portal.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/threat-intelligence.png)
To view a screen capture from each of the categories, select the tab from the image that follows. In each case, there's a side panel that shows the embedded Microsoft Security Copilot capability.![A screenshot of the threat analytics dashboard.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/threat-analytics.png)![A screenshot of the intel profiles page in threat intelligence.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/intel-profiles.png)![A screenshot of the intel explorer page in threat intelligence.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/intel-explorer.png)![A screenshot of the projects page in threat intelligence.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/projects.png)
### [[Microsoft Security Copilot]] integration with [[Microsoft Defender Threat Intelligence (Defender TI)]]
Security Copilot integrates with Microsoft Defender TI. With the Defender TI plugin enabled, Copilot delivers information about threat activity groups, indicators of compromise (IOCs), tools, and contextual threat intelligence. You can use the prompts and promptbooks to investigate incidents, enrich your hunting flows with threat intelligence information, or gain more knowledge about your organization's or the global threat landscape.

[[Microsoft Defender Threat Intelligence (Defender TI)]] capabilities in Copilot are built-in prompts that you can use, but you can also enter your own prompts based on the capabilities supported. The image that follows shows only a subset of the capabilities supported.![Screen capture of the Defender TI system capabilities that can be run in the standalone experience.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-threat-protection-with-microsoft-365-defender/media/copilot-capabilities.png)
Copilot also includes a builtin promptbook that deliver information from [[Microsoft Defender Threat Intelligence (Defender TI)]] including:
- Vulnerability impact assessment - Generates a report summarizing the intelligence for a known vulnerability, including steps on how to address it.
- Threat actor profile - Generates a report profiling a known activity group, including suggestions to defend against their common tools and tactics.

Copilot integration with Defender TI can also be experienced through the embedded experience. You can experience Security Copilot's capability to look up threat intelligence in the following pages of the Microsoft Defender portal:
- [[Threat analytics]]
- [[Intel profiles]]
- [[Intel explorer]]
- [[Intel projects]]
