- allows you to balance your organization's need for security & employee productivity with the right processes & visibility. As employees' role change within an organization, you can use [[Microsoft Entra ID Governance]] to automatically ensure that the right people have the right access to the right resources, with identity & access process automation, delegation to business groups & increased visibility.

ID governance gives organizations the ability to do the following tasks:
1. Govern the identity lifecycle
2. Govern access lifecycle
3. Secure privileged access for administration

These actions can be completed for employees, business partners & vendors & across services & applications, both on-premises & in the cloud

It's intended to help organizations address these 4 key questions
1. Which users should have access to which resources
2. What are those users doing with that access
3. Are there effective organizational controls for managing access
4. Can auditors verify that the controls are working
### Identity lifecycle
 ![Diagram showing identity lifecycle for employees. The lifecycle is represented as a circle that starts with no access followed by joining the organization then moving to a new role and then leaving the organization. The cycle repeats.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-identity-protection-governance-capabilities/media/2-identify-lifecycle-management-v3.png)
You can automate the identity lifecycle of users using:
1. Inbound provisioning from your organization's HR sources, to automatically maintain user identities in both [[Microsoft Entra ID]] & Active Directory
2. Lifecycle workflows to automate workflow tasks that run at certain key events, such before a new employee is schedule to start work at the organization, as they change status during their time in the organization & as they leave the organization
3. Automatic assignment policies in entitlement management to add & remove a user's group memberships, application roles, & SharePoint site roles, based on changes ot the user's attributes. Information on entitlement management is covered in a subsequent unit.
4. User provisioning to create, update & remove user accounts in other applications, with connectors to hundreds of cloud & on-premises applications.
In general, managing the lifecycle of an identity is about updating the access the users need, whether through integration with an HR system, or through user provisioning applications
### Access lifecycle
- the process of managing access throughout the user's organizational life. Users require different levels of access from the point at which they join an organization to when they leave it.
- With [[Microsoft Entra ID Governance]], IT departments can establish what access rights users should have across various resources and what enforcement checks are necessary

Organizations can automate the access lifecycle process through technologies such as [[Dynamic Groups]]. When any attributes of a user or device change, the system evaluates all dynamic group rules in a directory to see if the change would trigger any users to be added or removed from a group. If a user or device satisfies a rule for a group, they're added as a member of that group. If they no longer satisfy the rule, they're removed.

Entitlement management enables organizations to define how users request access across packages of group & team memberships, app roles & SharePoint Online roles & enforce separation of duties checks on access requests.

Organizations can regularly review access rights using recurring Microsoft Entra access reviews for access recertification.
### Privileged access lifecycle
Monitoring privileged access is a key part of identity governance. When employees, vendors & contractors are assigned administrative rights, there should be a governance process because of the potential for misuse.

Microsoft [[Privileged Identity Management (PIM)]] provides extra controls tailored to securing access rights. [[Privileged Identity Management (PIM)]] helps you minimize the number of people who have access to resources across [[Microsoft Entra ID]], Azure & other Microsoft online services. [[Privileged Identity Management (PIM)]] provides a comprehensive set of governance controls to help secure your company's resources.![Diagram showing the identity access rights lifecycle. The lifecycle is represented as a circle that starts with no admin followed a first admin role then a second admin role then leaving IT.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-identity-protection-governance-capabilities/media/privileged-access-lifecycle.png)