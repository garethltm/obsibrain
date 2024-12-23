Microsoft Entra logs all sign-ins into a Microsoft Entra tenant, which includes your internal apps and resources. The sign-in logs provided by [[Microsoft Entra ID]] are a powerful type of [activity log](https://learn.microsoft.com/en-us/entra/identity/monitoring-health/overview-monitoring-health) that you can analyze.
- [[Audit Logs]] – Information about changes applied to your tenant, such as users and group management or updates applied to your tenant’s resources.
- **[Provisioning](https://learn.microsoft.com/en-us/entra/identity/monitoring-health/concept-provisioning-logs)** – Activities performed by a provisioning service, such as the creation of a group in ServiceNow or a user imported from Workday.
### What can you do with sign-in logs
You can use the sign-in logs to answer questions such as:
- How many users signed into a particular application this week?
- How many failed sign-in attempts occurred in the last 24 hours?
- Are users signing in from specific browsers or operating systems?
- Which of my Azure resources were accessed by managed identities and service principals?

You can also describe the activity associated with a sign-in request by identifying the following details:
- **Who** – The identity (User) performing the sign-in.
- **How** – The client (Application) used for the sign-in.
- **What** – The target (Resource) accessed by the identity.
### What are the types of sign-in logs?
There are four types of logs in the sign-in logs preview:
- [Interactive user sign-ins](https://learn.microsoft.com/en-us/entra/identity/monitoring-health/concept-interactive-sign-ins)
- [Non-interactive user sign-ins](https://learn.microsoft.com/en-us/entra/identity/monitoring-health/concept-noninteractive-sign-ins)
- [Service principal sign-ins](https://learn.microsoft.com/en-us/entra/identity/monitoring-health/concept-service-principal-sign-ins)
- [Managed identity sign-ins](https://learn.microsoft.com/en-us/entra/identity/monitoring-health/concept-managed-identity-sign-ins)

Sign-in data is used by several services in Azure and Microsoft Entra to monitor risky sign-ins, provide insight into application usage, and more.

### Microsoft Entra Usage & Insights
- for application-specific sign-in data![Screenshot of the Usage & insights report.](https://learn.microsoft.com/en-us/entra/identity/monitoring-health/media/concept-sign-ins/usage-insights.png)
	There are several reports available in **Usage & insights**. Some of these reports are in preview.
	
	- Microsoft Entra application activity (preview)
	- AD FS application activity
	- Authentication methods activity
	- Service principal sign-in activity
	- Application credential activity

