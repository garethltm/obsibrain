Effective management of an organization’s network security perimeter requires the right combination of tools and systems. [[Microsoft Sentinel]] is a scalable, cloud-native SIEM/SOAR solution that delivers intelligent security analytics and threat intelligence across the enterprise. It provides a single solution for cyberthreat detection, investigation, response, and proactive hunting, with a bird's-eye view across your enterprise.![Diagram showing the four aspects of Microsoft Sentinel: collect, detect, investigate, and respond.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-security-capabilities-of-azure-sentinel/media/3-four-aspects-azure-sentinel.png)This diagram depicts the end-to-end functionality of Microsoft Sentinel.

- **Collect** data at cloud scale across all users, devices, applications, and infrastructure, both on-premises and in multiple clouds.
- **Detect** previously uncovered threats and minimize false positives using analytics and unparalleled threat intelligence.
- **Investigate** threats with artificial intelligence (AI) and hunt suspicious activities at scale, tapping into decades of cybersecurity work at Microsoft.
- **Respond** to incidents rapidly with built-in orchestration and automation of common security tasks.

Microsoft Sentinel helps enable end-to-end security operations, in a modern Security Operations Center (SOC).
### Collect data at scale
Collect data across all users, devices, applications, and infrastructure, both on-premises and in multiple clouds. The following are key capabilities in [[Microsoft Sentinel]] for data collection.

- _**Out of the box data connectors**_
	- Many connectors are packaged with SIEM solutions for Microsoft Sentinel and provide real-time integration. These connectors include Microsoft sources and Azure sources like [[Microsoft Entra ID]], Azure Activity, Azure Storage, and more.
	- Out of the box connectors are also available for the broader security and applications ecosystems for non-Microsoft solutions. You can also use common event format, Syslog, or REST-API to connect your data sources with [[Microsoft Sentinel]].
    
- _**Custom connectors**_
	- [[Microsoft Sentinel]] supports ingesting data from some sources without a dedicated connector. If you're unable to connect your data source to [[Microsoft Sentinel]] using an existing solution, you can create your own data source connector.
    
- _**Data normalization**_
	- [[Microsoft Sentinel]] ingests data from many sources. Working with and correlating between different types of data during an investigation and hunting can be challenging. [[Microsoft Sentinel]] supports the Advanced Security Information Model (ASIM), that sits between these diverse sources and the user, to facilitate uniform, normalized views.
### Detect threats
Detect previously undetected threats, and minimize false positives using Microsoft's analytics and unparalleled threat intelligence. The following are key capabilities in [[Microsoft Sentinel]] for threat detection.

- _**Analytics**_ 
	- [[Microsoft Sentinel]] uses analytics to group alerts into incidents. Use the out of the box analytic rules as-is, or as a starting point to build your own rules. [[Microsoft Sentinel]] also provides rules to map your network behavior and then look for anomalies across your resources.
    
- _**MITRE ATT&CK coverage**_
	- [[Microsoft Sentinel]] analyzes ingested data, not only to detect threats and help you investigate, but also to visualize the nature and coverage of your organization's security status based on the tactics and techniques from the MITRE ATT&CK® framework, a global database of adversary tactics and techniques.
    
- _**Threat intelligence**_ - You can integrate numerous sources of threat intelligence into Microsoft Sentinel to detect malicious activity in your environment and provide context to security investigators for informed response decisions.
    
- _**Watchlists**_ - You can correlate data from a data source you provide, a watchlist, with the events in your Microsoft Sentinel environment. For example, you might create a watchlist with a list of high-value assets, terminated employees, or service accounts in your environment. Use watchlists in your search, detection rules, threat hunting, and response playbooks.
    
- _**Workbooks**_ - You can create interactive visual reports by using workbooks. After you connect data sources to Microsoft Sentinel, you can monitor the data using the Microsoft Sentinel integration with Azure Monitor Workbooks. Microsoft Sentinel comes with built-in workbook templates that allow you to quickly gain insights across your data. You can also create your own custom workbooks.