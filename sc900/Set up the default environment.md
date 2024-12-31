To set up the default environment, you need ot have one of the following [[Microsoft Entra ID]] roles:
1. Global administrator
2. Security administrator

During the setup of Security Copilot, you're prompted to configure settings. These include:

- [[Security Compute Unit (SCU)]] capacity - Select the capacity of [[Security Compute Unit (SCU)]](s) previously provisioned.
    
- Data storage - When an organization onboards to Copilot, the admin must confirm the geographic location of the tenant as the customer data collected by the services is stored there. Microsoft Security Copilot operates in the Microsoft Azure data centers in the European Union (EUDB), the United Kingdom, the United States, Australia and New Zealand, Japan, Canada, and South America.
    
- Decide where your [[Prompt]](s) are evaluated - You can restrict the evaluation within your geo or allow evaluation anywhere in the world.
    
- Logging audit data in [[Microsoft Purview]] - As part of the initial setup and listed under Owner settings in the standalone experience, you can choose to allow [[Microsoft Purview]] to process and store admin actions, user actions, and Copilot responses. This includes data from any Microsoft and non-Microsoft Integrations. If you opt in and you already use [[Microsoft Purview]], no further action is needed. If you opt in but aren't already using Purview, you need to follow the [[Microsoft Purview]] guides to set up a limited experience.![Screen capture showing the settings for how you can configure audit logging.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/owner-settings-logging-audit-data.png)
- Your organization's data - The admin must also opt in or opt out of data sharing options. These options are part of the initial setup and also listed under Owner settings in the standalone experience. Turn the toggles on or off for any of the following options:
	- Allow Microsoft to capture data from Security Copilot to validate product performance using human review: When turned on, customer data is shared with Microsoft for product improvement. Prompts and responses are evaluated to understand whether the right plugins were selected, if the output is what was expected, how responses, latency, and output format can be improved.
	- Allow Microsoft to capture and human review data from Security Copilot to build and validate Microsoft's security AI model: When turned on, customer data is shared with Microsoft for Copilot AI improvement. Opting in does NOT allow Microsoft to use customer data to train foundational models. Prompts and responses are evaluated to enhance responses and to ensure they're what's expected and useful to you.![Screen capture showing the settings for how you can configure data sharing to help improve Copilot.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/help-improve-copilot.png)
	- Plugin settings - The admin manages plugins and configures whether to allow Security Copilot to access data from your Microsoft 365 services.
		- Configure who can add and manage their own custom plugins and who can add and manage custom plugins for everyone in the organization.
		- Manage plugin availability and restrict access. When enabled, admins decide which new and existing plugins will be available to everyone in your organization, and which will be restricted to owners only.
		- Allow Security Copilot to access data from your Microsoft 365 services. If this option is turned off, your organization won't be able to use plugins that access Microsoft 365 services. Currently, this option is required for use of the Microsoft Purview plugin. Setting and/or changing this setting requires a user with a Global administrator role.![Screen capture showing the plugin settings and the setting to allow Security Copilot to access data from your Microsoft 365 services.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/plugin-settings-no-restrictions.png)
### Role permissions
To ensure that the users can access the features of Copilot, they need to have the appropriate role permissions.

Permissions can be assigned using [[Microsoft Entra ID]] roles or Security Copilot roles. As a best practice, provide the least privileged role applicable for each user.

The [[Microsoft Entra ID]] roles are:
- Global administrator
- Security administrator
- Security operator
- Security reader

Although these [[Microsoft Entra ID]] roles grant users varying levels of access to Copilot, the scope of these roles extends beyond Copilot. For this reason, Security Copilot introduces two roles that function like access groups but aren't [[Microsoft Entra ID]] roles. Instead, they only control access to the capabilities of the Security Copilot platform.

The [[Microsoft Security Copilot]] roles are:
- Copilot owner
- Copilot contributor

The Security Administrator and Global Administrator roles in Microsoft Entra automatically inherit Copilot owner access.![Screen capture showing the role assignment settings.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/role-assignments-new-edited.png)
Only users that have the global administrator, security administrator, or Copilot owner roles can make role assignments in Copilot by adding/removing members from the Owner and Contributor roles.

A group that admins/owners can include as a member of the Contributor role is the **Recommended Microsoft Security roles** group. This group exists only in Security Copilot and is a bundle of existing Microsoft Entra roles. When you add this group as a member of the Contributor role, all users that are members of the [[Microsoft Entra ID]] roles that are included in the recommended Microsoft Security roles group get access to the Copilot platform. This option provides a quick, secure way to give users in your organization, who already have access to security data used by Copilot through a Microsoft plugin, access to the Copilot platform.
