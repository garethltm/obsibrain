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
    
- _**[[MITRE ATT&CK]] coverage**_
	- [[Microsoft Sentinel]] analyzes ingested data, not only to detect threats and help you investigate, but also to visualize the nature and coverage of your organization's security status based on the tactics and techniques from the [[MITRE ATT&CK]]® framework, a global database of adversary tactics and techniques.
    
- _**Threat intelligence**_
	- You can integrate numerous sources of threat intelligence into [[Microsoft Sentinel]] to detect malicious activity in your environment and provide context to security investigators for informed response decisions.
    
- _**Watchlists**_
	- You can correlate data from a data source you provide, a watchlist, with the events in your [[Microsoft Sentinel]] environment. 
		>For example, you might create a watchlist with a list of high-value assets, terminated employees, or service accounts in your environment. Use watchlists in your search, detection rules, threat hunting, and response playbooks.
    
- _**Workbooks**_
	- You can create interactive visual reports by using workbooks. After you connect data sources to [[Microsoft Sentinel]], you can monitor the data using the [[Microsoft Sentinel]] integration with Azure Monitor Workbooks. [[Microsoft Sentinel]] comes with built-in workbook templates that allow you to quickly gain insights across your data. You can also create your own custom workbooks.
### Investigate threats
Investigate threats with [[Artificial Intelligence (AI)]], and hunt for suspicious activities at scale, tapping into years of cyber security work at Microsoft. The following are key capabilities in [[Microsoft Sentinel]] for threat investigation.

- _**Incidents**_
	- Incidents are your case files that contain an aggregation of all the relevant evidence for specific investigations. Each incident is created (or added to) based on pieces of evidence (alerts) that were either generated by analytics rules or imported from third-party security products that produce their own alerts. The incident details page provides information and investigation tools to help you to understand the scope and find the root cause of a potential security threat.
    
- _**Hunts**_
	- [[Microsoft Sentinel]]'s powerful hunting search-and-query tools, based on the [[MITRE ATT&CK]] framework, enable you to proactively hunt for security threats across your organization’s data sources, before an alert is triggered. After you discover which hunting query provides high-value insights into possible attacks, you can also create custom detection rules based on your query, and surface those insights as alerts to your security incident responders.
    
- _**Notebooks**_
	- [[Microsoft Sentinel]] supports Jupyter notebooks in Azure Machine Learning workspaces. Jupyter notebooks are an open-source web application that allows users to create and share documents containing live code, equations, visualizations, and narrative text.
    
	    Use notebooks in Microsoft Sentinel to extend the scope of what you can do with Microsoft Sentinel data. For example:
	    - Perform analytics that aren't built in to [[Microsoft Sentinel]], such as some Python machine learning features.
	    - Create data visualizations that aren't built in to [[Microsoft Sentinel]], such as custom timelines and process trees.
	    - Integrate data sources outside of [[Microsoft Sentinel]], such as an on-premises data set.
### Respond to incidents rapidly
With [[Microsoft Sentinel]], you can automate your common tasks and simplify security orchestration with playbooks that integrate with Azure services and your existing tools, to respond to incidents more rapidly.

The following are key capabilities in Microsoft Sentinel for threat response.
- _**Automation rules**_
	- Centrally manage the automation of incident handling in [[Microsoft Sentinel]] by defining and coordinating a small set of rules that cover different scenarios.
- _**Playbooks**_
	- Automate and orchestrate your threat response by using playbooks, which are a collection of remediation actions. Run a playbook on-demand or automatically in response to specific alerts or incidents, when triggered by an automation rule. Playbooks in [[Microsoft Sentinel]] are based on workflows built in Azure Logic Apps. For example, if you use the ServiceNow ticketing system, use Azure Logic Apps to automate your workflows and open a ticket in ServiceNow each time a particular alert or incident is generated.
### Enable out of the box security conent
