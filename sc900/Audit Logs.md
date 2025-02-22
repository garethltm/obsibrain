Audit logs in [[Microsoft Entra ID]] provide access to system activity records, often needed for compliance. You can get answers to questions related to users, groups, and applications.

**Users:**
- What types of changes were recently applied to users?
- How many users were changed?
- How many passwords were changed?

**Groups:**
- What groups were recently added?
- Have the owners of group been changed?
- What licenses are to a group or a user?

**Applications:**
- What applications were, updated, or removed?
- Has a service principal for an application changed?
- Have the names of applications been changed?

**Custom security attributes:**
- What changes were made to [custom security attribute](https://learn.microsoft.com/en-us/entra/fundamentals/custom-security-attributes-overview) definitions or assignments?
- What updates were made to attribute sets?
- What custom attribute values were assigned to a user?

## What do the logs show
- Date and time of the occurrence
- Service that logged the occurrence
- Category and name of the activity (_what_)
- Status of the activity (success or failure)
![Screenshot of the audit logs, with the Directory and Custom Security tabs highlighted.](https://learn.microsoft.com/en-us/entra/identity/monitoring-health/media/concept-audit-logs/audit-log-tabs.png)