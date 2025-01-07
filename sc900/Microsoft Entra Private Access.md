- provides your users, whether in an office or working remote remotely secure access to your private, corporate resources
- can be deployed to block lateral attack movement, reduce excessive access & replace legacy VPNs.
## 1. Quick Access
- works by creating a new enterprise application that serves as a container for the private resources you want to secure![Diagram of Microsoft Entra Private Access with showing the components of Quick Access.](https://learn.microsoft.com/en-us/training/wwl-sci/explore-access-management-capabilities/media/quick-access-diagram.png)
- you can determine which private resources to add to the "container" or enterprise application; defined by "**Quick Access application**"
	- the private resources you add to the "**Quick Access application**" are defined by the [[Fully Qualified Domain Name (FQDN)]], IP address, IP or address range & ports used to access the resource.
		- This information is referred to as a "**Quick Access application**" segment.
		- You can add many application segments to the "**Quick Access application**".
		- You can then link [[conditional access]] policies to the "**Quick Access application**"
## 2. [[Global Secure Access]] app (Per-app Access)
- more granular approach
- you can create multiple "containers" or enterprise application.
- For each of these new enterprise apps, you define the properties of the private resource & you assign users & groups & assign specific [[conditional access]] policies![Diagram of Microsoft Entra Private Access with showing the components of Global Secure Access app, also referred to as Per-app Access.](https://learn.microsoft.com/en-us/training/wwl-sci/explore-access-management-capabilities/media/per-app-access-diagram.png)