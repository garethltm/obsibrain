- basically if-then statements
	- if user wants to access a resource they must complete an action![Diagram showing concept of Conditional Access signals plus decision to enforce organizational policy.](https://learn.microsoft.com/en-us/entra/identity/conditional-access/media/common-conditional-access-media/conditional-access-signal-decision-enforcement.png)
- a feature of [[Microsoft Entra ID]] that provides an extra layer of security before allowing authenticated users to access data or other assets
~ Use [[Conditional Access]] policies 
	1. to apply the right access controls when needed to keep it secure
	2. to enforce organizational rules for access

Access policy analyses signals including user, location, device, application & risk to automate decisions for authorizing access to resources (apps & data)
![Screenshot showing Conditional Access policy flow. Signals are used to decide whether to allow or block access to apps and data.](https://learn.microsoft.com/en-us/training/wwl-sci/explore-access-management-capabilities/media/conditional-access.png)

## Components
1. assignments
2. access controls
	![Screen capture showing the two components of a conditional access policy, the assignments and the access controls.](https://learn.microsoft.com/en-us/training/wwl-sci/explore-access-management-capabilities/media/conditional-access-policy-components-v3.png)
### Assignments
- logically an AND-statement
	- if you have more than 1 assignment configured (all assignments must be satisfied to trigger a policy)
### Access controls
- an informed decision is reached whether to
	- block access
	- grant access
	- grant access with extra verification
	- apply a session control to enable a limited experience


