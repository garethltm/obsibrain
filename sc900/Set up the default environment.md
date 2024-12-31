To set up the default environment, you need ot have one of the following [[Microsoft Entra ID]] roles:
1. Global administrator
2. Security administrator

During the setup of Security Copilot, you're prompted to configure settings. These include:

- [[Security Compute Unit (SCU)]] capacity - Select the capacity of [[Security Compute Unit (SCU)]](s) previously provisioned.
    
- Data storage - When an organization onboards to Copilot, the admin must confirm the geographic location of the tenant as the customer data collected by the services is stored there. Microsoft Security Copilot operates in the Microsoft Azure data centers in the European Union (EUDB), the United Kingdom, the United States, Australia and New Zealand, Japan, Canada, and South America.
    
- Decide where your [[Prompt]](s) are evaluated - You can restrict the evaluation within your geo or allow evaluation anywhere in the world.
    
- Logging audit data in [[Microsoft Purview]] - As part of the initial setup and listed under Owner settings in the standalone experience, you can choose to allow [[Microsoft Purview]] to process and store admin actions, user actions, and Copilot responses. This includes data from any Microsoft and non-Microsoft Integrations. If you opt in and you already use Microsoft Purview, no further action is needed. If you opt in but aren't already using Purview, you need to follow the Microsoft Purview guides to set up a limited experience.