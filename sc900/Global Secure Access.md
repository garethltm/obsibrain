- a unifying term used for both [[Microsoft Entra Internet Access]] & [[Microsoft Entra Private Access]]

The solution employs a [[Global Secure Access]] client that gives organizations control over network traffic at the end-user computing device. Organizations gain the ability to route specific traffic profile through [[Microsoft Entra Internet Access]] & [[Microsoft Entra Private Access]]. 
![Screenshot showing components that make up Global Secure Access.](https://learn.microsoft.com/en-us/training/wwl-sci/explore-access-management-capabilities/media/global-secure-access-v3.png)
- Routing traffic in this method allows for more controls enabled by deep integration with [[Conditional Access]] policies & risks assessed in real time, across identity, device, location & applications to protect any app or resource.
## Dashboard
- provides you with visualizations of the network traffic acquired by the [[Microsoft Entra Private Access]] & [[Microsoft Entra Internet Access]] services. The dashboard compiles the data from your network configurations, including devices, users & tenants into several widgets. Those widgets, in turn, provide you with information you can use to monitor & improve your network configurations.
1. Global Secure Access snapshot
	- provides a summary of how many users & devices are using the service & how many applications were secured through the service![Screenshot of the Global Secure Access snapshot widget.](https://learn.microsoft.com/en-us/training/wwl-sci/explore-access-management-capabilities/media/global-secure-access-snapshot-widget.png)
	- The widget defaults to showing all types of traffic but you can change the filter to show Internet Access, Private Access or Microsoft traffic
2. Usage profiling (preview)
	- The Usage profiling widget displays usage patterns for Internet Access, Private Access or Microsoft 365 over a selected period of time & by category![Screenshot of the usage profiling widget.](https://learn.microsoft.com/en-us/training/wwl-sci/explore-access-management-capabilities/media/dashboard-usage-profiling.png)
3. Alerts & notifications (preview)
	- The Alerts & notifications widget shows what is happening in the network & helps identify suspicious activities or trends identified by the network data
	- Widgets:
		1. Unhealthy remote network - An unhealthy remote network has 1 or more device links disconnected
		2. Increased external tenants activity - The number of users accessing external tenants has increased
		3. Token & device inconsistency - The original token is used on a different device
		4. Web content blocked - Access to the website has been blocked![Screenshot of the dashboard alerts notifications widget.](https://learn.microsoft.com/en-us/training/wwl-sci/explore-access-management-capabilities/media/dashboard-alerts-notifications.png)
4. Cross tenant access
	- [[Global Secure Access]] provides visibility into the number of users & devices that are accessing other tenants.
	- Widgets:
		1. Sign-ins - The number of sign-ins through [[Microsoft Entra ID]] to Microsoft services in the last 24 hours. This widget provides you with information about the activity in your tenant
		2. Total distinct tenants - The number of distinct tenant IDs seen in the last 24 hours
		3. Unseen tenants - The number of distinct tenants