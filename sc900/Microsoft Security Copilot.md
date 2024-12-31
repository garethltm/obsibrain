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
1. Investigate & remediate security threats - gain context for incidents to quickly triage complex security alerts into actionable summaries & remediate quicker with step-by-step response guidance.
2. Build KQL queries or analyze suspicious scripts - eliminate the need to manually write query-language scripts or reverse engineer malware scripts with natural language translation to enable every team member to execute technical tasks
3. Understand risks & manage security posture of the organization - get a broad picture of your environment with prioritized risks to uncover opportunities to improve posture more easily
4. Troubleshoot IT issues faster - synthesize relevant information rapidly & receive actionable insights to identify & resolve IT issues quickly
5. Define & manage security policies - define a new policy, cross-reference it with others for conflicts, & summarize existing policies to manage complex organization context quickly & easily
6. Configure secure lifecycle workflows - build groups & set access parameters with step-by-step guidance to ensure a seamless configuration to prevent security vulnerabilities
7. Develop reports for stakeholders - get a clear & concise report that summarizes the context & environment, open issues & protective measures prepared for the tone & language of the report's audience
### Standalone & embedded experience
1. Dedicated site (standalone experience)![Screenshot that shows the landing page for the Security Copilot standalone experience. The prompt bar is at the bottom center of the page.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/copilot-landing-page-prompt-bar.png)
2. Embedded experience through Microsoft Security products![Diagram that shows the advanced hunting page of Microsoft Defender XDR, The page includes a button for Copilot that When selected opens a side panel for natural language to KQL query assistant.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/security-copilot-embedded-m365-xdr-v3.png)

Copilot is built using Azure OpenAI Services & is designed to integrate with existing security tools & processes, making it easier for organizations to improve their overall security posture. Azure OpenAI Services provides REST API access to OpenAI's powerful large language models (LLMs) for [[Natural Language Processing (NLP)]], while providing security capabilities of Microsoft Azure.

With access to the powerful LLMs for [[Natural Language Processing (NLP)]], Copilot is able to read, decipher & make sense of human languages, enabling users to securely interact with it using natural language. Although the LLMs are trained on a vast amount of information that endows Copilot with broad general knowledge and problem solving abilities, it’s not enough. Security analysts expect their copilot to be trained on security and that is where the integration with existing security tools and processes comes into play.
### Integration with Security-specific sources
Copilot combines powerful LLMs with security-specific sources from Microsoft. These security-specific sources are informed by Microsoft’s unique global threat intelligence, more than 65 trillion daily signals, and incorporates information from a growing set of security solutions using plug-ins and connections to knowledge bases. Through plug-ins, Copilot integrates with Microsoft's own security products, non-Microsoft products, and open-source intelligence feeds. Connections to an organization's knowledge bases gives Copilot more context, resulting in responses that are more relevant, specific, and customized to the user. Through the powerful combination of advanced general models and security specific sources, Copilot is able to learn at machine speed to help analysts identify and respond to emerging threats.

The information you give Copilot will only be accessible to your organization. Your data is your data, and it's protected by comprehensive enterprise compliance and security controls. Your data isn't used to train the foundation AI models.![Diagram showing key attributes of Security Copilot, including hyperscale AI infrastructure, security specific orchestrator,evergreen threat intelligence, and cyber skills and promptbooks.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/security-copilot-v2.png)
## Terminology
- [[sc900/Session|Session]]
- [[Prompt]]
- [[Capability]]
- [[Plugin]]
- [[Orchestrator]]

### Prompt bar & [[sc900/Session|Session]]
- At the center of Security Copilot is the prompt bar. You use the prompt bar to tell Copilot what insights you want from your security data, this is referred to as the [[prompt]]. In other words, the [[prompt]] is the text-based, natural language input you provide in the prompt bar that instructs Copilot to generate a response. Although you interact with Copilot in natural language, it’s helpful to be specific in the [[Prompt]](s) (specific questions or statements) that you provide. For those that are relatively new to the security analyst role and engaging with AI, effective prompting may take some practice. For this reason, Copilot provides promptbooks that provide a series of preselected prompts and prompt suggestions (more details on this in a subsequent module).![A screen capture of the Microsoft Security Copilot prompt bar.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/prompt-bar-new.png)
### Plugins & capabilities
In the previous unit, we mentioned that Copilot integrates with various sources through [[Plugin]](s), including Microsoft's own security products such as Microsoft Sentinel, Microsoft Defender XDR, and Microsoft Intune, non-Microsoft solutions, and open-source intelligence feeds. The integration enabled by the plugin, for any specific data source, provides Copilot with a collection of capabilities. Each [[capability]] is like a function in software, it’s designed to do a specialized task within the scope of the data source. 

> #Example the plugin to Microsoft Defender XDR includes a collection of individual capabilities that are used only by Microsoft Defender XDR. These include:
> 	- The ability to summarize an incident.
> 	- Support incident response teams in resolving incidents through guided responses (a set of recommended actions based on the specific incident).
> 	- The ability to analyze scripts and code.
> 	- The ability to generate KQL queries from natural language input.
> 	- The ability to generate incident reports.

A [[plugin]] for Microsoft Sentinel may have similar capabilities but runs only within the scope of Microsoft Sentinel.

Copilot currently supports plug-ins for Microsoft services and non-Microsoft services, including websites and custom plug-ins that can be enabled.![A screen capture of the plugins window, showing the Microsoft plugins, including Entra, Intune, Microsoft Defender XDR, and more.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/microsoft-plugins-updated.png)![A screen capture of the plugins window, showing the non-Microsoft plugins, including ServiceNow, Splunk, the public web, and custom plugins.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/non-microsoft-plugins-updated.png)
## Process flow
When a user submits a [[prompt]], Copilot processes that prompt to generate the best possible response. The diagram that follows illustrates, at a high level, steps that Copilot takes to process the [[prompt]] and generate a response.![Diagram illustrating how Microsoft Security Copilot processes a prompt request.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/copilot-how-it-works-v2.png)
1. Submit a [[prompt]]: The process starts when a user submits a [[prompt]] in the prompt bar.
    
2. [[Orchestrator]]: Security Copilot sends the information to the Copilot backend referred to as the [[orchestrator]]. The [[orchestrator]] is Copilot’s system for composing [[Capability]](s) together to answer a user’s [[prompt]]. It determines the initial context and builds a plan using all the available [[Capability]](s) (skills).
    
3. Build context: Once a plan is defined and built, Copilot executes that plan to get the required data context to answer the [[prompt]].
    
4. [[Plugin]](s): In the course of executing the plan, Copilot analyzes all data and patterns to provide intelligent insights. This includes reasoning over all the [[Plugin]](s) and sources of data, enabled and available to Copilot.
    
5. Responding: Copilot combines all the data and context and uses the power of its advanced LLM to compose a response using language that makes sense to a human being.
    
6. Response: Before the response can be sent back to the user, Copilot formats and reviews the response as part of Microsoft's commitment to responsible AI.
    
7. Receives response: The process culminates with the user receiving the response from the Copilot.
### Process log
During this process, Copilot generates a process log that is visible to the user. The user can see what [[capability]] is used to generate the response. This is important because it enables the user to determine whether the response was generated from a trusted source. In the screenshot that follows, the process log shows that Copilot chose the Incident Analysis capability. The process log also shows that the final output went through safety checks, which is part of Microsoft’s commitment to responsible AI.![Screen capture of the process log that highlights the capability selected and the text indicating that Copilot ran safety checks as part of the process to compose the response message.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/process-log-new.png)
## Steps to onboard the service & users
1. [[Provision Copilot capacity]]
2. Set up the default environment
3. Assign role permissions