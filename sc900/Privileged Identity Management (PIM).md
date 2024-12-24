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
- reduces the chance of a malicious actor getting access by minimizing the number of people who have access to secure information or resources. By time-limiting authorized users, it reduces the risk of an authorized user inadvertently affecting sensitive resources. [[Privileged Identity Management (PIM)]]

Supports all roles currently in Azure [[Active Directory (AD)]]
![[Pasted image 20241219131303.png]]

& Azure Resource Roles (Azure Resources)
## General workflow
