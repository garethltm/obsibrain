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