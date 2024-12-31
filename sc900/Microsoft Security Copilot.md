- [[Microsoft Entra ID]] integrates with [[Microsoft Security Copilot]]

Business that are onboarded to Copilot & whose users have the appropriate role permissions can take advantage of this integration by enabling the Microsoft Entra plugin
![Screen capture of the Entra plugin in Microsoft Security Copilot.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-identity-protection-governance-capabilities/media/entra-plugin.png)
- With the Entra plugin enabled, security analysts can instantly get 
	- a risk summary
	- steps to remediate
	- recommended guidance for each identity at risk

Analysts can use Copilot to guide in the creation of a lifecycle workflow to streamline the process of creating & issuing user credentials & access rights. These & many other Entra capabilities are supported by Copilot

[[Microsoft Entra ID]] capabilities in Copilot are built-in prompts that you can use but you can also enter your own prompts based on the capabilities supported![Screen capture of the Entra capabilities that can be run in the standalone experience.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-identity-protection-governance-capabilities/media/entra-skills.png)

Microsoft Entra integration with Copilot can also be experienced through embedded experience, referred to as Microsoft Copilot in [[Microsoft Entra ID]]

> #Example the risky user's report, available from the Microsoft Entra admin center under Identity protection, embeds the capabilities of [[Microsoft Security Copilot]] to summarize a user's risk level, provide insights relevant to the incident at hand, & provide recommendations for rapid mitigation
![Screen capture showing the Copilot generated summary.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-identity-protection-governance-capabilities/media/entra-risky-users-summarize-v2.png)
## Use cases
- Investigate & remediate security threats - gain context for incidents to quickly triage complex security alerts into actionable summaries & remediate quicker with step-by-step response guidance.
- Build KQL queries or analyze suspicious scripts - eliminate the need to manually write query-language scripts or reverse engineer malware scripts with natural language translation to enable every team member to execute technical tasks
- Understand risks & manage security posture of the organization - get a broad picture of your environment with prioritized risks to uncover opportunities to improve posture more easily
- Troubleshoot IT issues faster - synthesize relevant information rapidly & receive actionable insights to identify & resolve IT issues quickly
- Define & manage security policies - define a new policy, cross-reference it with others for conflicts, & summarize existing policies to manage complex organization context quickly & easily
- Configure secure lifecycle workflows - build groups & set access parameters with step-by-step guidance to ensure a seamless configuration to prevent security vulnerabilities
- Develop reports for stakeholders - get a clear & concise report that summarizes the context & environment, open issues & protective measures prepared for the tone & language of the report's audience
### Standalone & embedded experience
1. Dedicated site (standalone experience)![Screenshot that shows the landing page for the Security Copilot standalone experience. The prompt bar is at the bottom center of the page.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/copilot-landing-page-prompt-bar.png)
2. Embedded experience through Microsoft Security products![Diagram that shows the advanced hunting page of Microsoft Defender XDR, The page includes a button for Copilot that When selected opens a side panel for natural language to KQL query assistant.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/security-copilot-embedded-m365-xdr-v3.png)

Copilot is built using Azure OpenAI Services & is designed to integrate with existing security tools & processes, making it easier for organizations to improve their overall security posture. Azure OpenAI Services provides REST API access to OpenAI's powerful large language models (LLMs) for [[Natural Language Processing (NLP)]], while providing security capabilities of Microsoft Azure.

With access to the powerful LLMs for [[Natural Language Processing (NLP)]], Copilot is able to read, decipher & make sense of human languages, enabling users to securely interact with it using natural language. Although the LLMs are trained on a vast amount of information that endows Copilot with broad general knowledge and problem solving abilities, it’s not enough. Security analysts expect their copilot to be trained on security and that is where the integration with existing security tools and processes comes into play.
### Integration with Security-specific sources
Copilot combines powerful LLMs with security-specific sources from Microsoft. 