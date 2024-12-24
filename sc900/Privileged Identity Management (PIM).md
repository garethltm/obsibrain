- Manage, control & monitor access to important resources
	- Provide **just in time (JIT)** privileged access to resources and directory
		- usually between 0-24 hours
	- Assign **time-bound access** to resources using start/end dates
	- Require **approval** to activate [[privileged roles]]
	- Enforce **MFA** to activate any role ([[sc900/Authentication|Authentication]])
	- Use **justification** to understand why users activate
	- Get **notifications** when privileged roles are activated
	- Conduct **Access Reviews** to ensure users still need roles
	- Download **audit history** for internal/external audit
![[Pasted image 20241219130311.png]]
## Reasons to use
- useful in a Guest scenario
	- maybe like an intern or something (2 months period for example)
- reduces the chance of a malicious actor getting access by minimizing the number of people who have access to secure information or resources. By time-limiting authorized users, it reduces the risk of an authorized user inadvertently affecting sensitive resources. [[Privileged Identity Management (PIM)]] also provides oversight for what users are doing with their administrator privileges.

Supports all roles currently in Azure [[Active Directory (AD)]]
![[Pasted image 20241219131303.png]]

& Azure Resource Roles (Azure Resources)
## General workflow
1. Assign
	- the assignment process starts by assigning roles to members. To grant access to a resource, the administrator assigns roles to users, groups, service principals or managed identities. Assignment includes:
		- Members or owners - the members or owners to assign to the role
		- Scope - the scope limits the assigned role to a particular set of resources
		- Assignment types:
			1. Eligible assignments require the member of the role to perform an action to use the role; Actions might include activation or requesting approval from designated approvers.
			2. Active assignments don't require the member to perform any action to use the role; Members assigned as active have the privileges assigned to the role.
		- Duration - the duration of the assignment is defined by start & end dates or is set to permanent.![Screen capture showing the assignment step.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-identity-protection-governance-capabilities/media/role-assignment-inline.png)
2. Activate
	- if users have been made eligible for a role, then they must activate the role assignment before using the role. To activate the role, users select specific activation duration within the maximum (configured by administrators) & the reason for the activation request![Screen capture showing the activation step.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-identity-protection-governance-capabilities/media/role-activation-inline.png)
3. Approve/Deny
	- Delegate approvers receive email notifications when a role request
4. Extend and renew