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
	- Microsoft Sentinel ingests data from many sources. Working with and correlating between different types of data during an investigation and hunting can be challenging. Microsoft Sentinel supports the Advanced Security Information Model (ASIM), that sits between these diverse sources and the user, to facilitate uniform, normalized views.