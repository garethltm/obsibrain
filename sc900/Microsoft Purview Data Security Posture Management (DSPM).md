allows you to quickly and easily monitor cross-cloud data and user risk through dynamic reports and trend analysis. By processing and correlating across other Microsoft Purview data security and risk and compliance solutions, DSPM (preview) helps you identify vulnerabilities with unprotected data and quickly take action to help you improve your data security posture and minimize risk. DSPM (preview) provides:

- **Data security recommendations**: 
	- Gain insights into your data security posture and get recommendations for creating insider risk management and data loss prevention (DLP) policies to help protect sensitive data and to close data security gaps. 
	>	For example, some recommendations may include creating policies to prevent users from printing sensitive files or to prevent users from copying sensitive files to other network locations.
- **Data security analytic trends and reports**: 
	- Track your organization's data security posture over time with reports summarizing sensitivity label usage, DLP policy coverage, changes in risky user behavior, and more.
- **Microsoft Security Copilot**: 
	- Use [[Microsoft Security Copilot]] to help you investigate alerts, identify risk patterns, and pinpoint the top data security risks in your organization.
### Integration with Microsoft Purview solutions
[[Microsoft Purview Data Security Posture Management (DSPM)]] (preview) processes and correlates data state, signals, and user activities based on the current configuration of other data security and risk and compliance solutions in Microsoft Purview. For optimal coverage and deeper insights, consider using the features and capabilities of the following solutions:

- **Data loss prevention (DLP)**: [Microsoft Purview Data Loss Prevention](https://learn.microsoft.com/en-us/purview/dlp-learn-about-dlp) policies help you prevent users from inappropriately sharing sensitive data. DLP detects sensitive information using content analysis that includes keyword matching, evaluations of expressions, internal validation, machine learning algorithms and more.
    
    Depending on specific recommendations identified for the data, you can choose to quickly create an applicable [DLP policy](https://learn.microsoft.com/en-us/purview/dlp-policy-design) directly in the DSPM (preview) workflow.
    
- **Information protection**: [Microsoft Purview Information Protection](https://learn.microsoft.com/en-us/purview/information-protection) provides a framework, process, and capabilities you can use to protect sensitive data across clouds, apps, and devices. Using sensitivity labels, trainable classifiers, and sensitive information types, organizations can define and apply protection policies to sensitive data.
    
- **Insider risk management**: [Microsoft Purview Insider Risk Management](https://learn.microsoft.com/en-us/purview/insider-risk-management) uses the full breadth of built-in service and 3rd-party indicators to help you quickly identify, triage, and act on potentially risky activity by users in your organization. By using logs from Microsoft 365 and Microsoft Graph, insider risk management allows you to define specific policies to identify risk indicators. After identifying the risks, you can take action to mitigate these risks, and if necessary open investigation cases and take appropriate legal action.
    
    Depending on specific recommendations identified for the data, you can choose to quickly create an applicable [insider risk management policy](https://learn.microsoft.com/en-us/purview/insider-risk-management-policy-templates) directly in the DSPM (preview) workflow.
### Working with Adaptive Protection
[Adaptive protection](https://learn.microsoft.com/en-us/purview/insider-risk-management-adaptive-protection) in Microsoft Purview uses [[Machine Learning (ML)]] to identify the most critical risks and proactively and dynamically apply protection controls from data loss prevention, data lifecycle management, and Microsoft Entra [[conditional access]]. If Adaptive Protection isn't currently enabled for unprotected sensitive data, you can create a new Adaptive Protection policy directly in the DSPM (preview) workflow.
## Workflow
The DSPM (preview) workflow helps you investigate and take action to address potential security concerns with unprotected data across your organization.![Data security posture management workflow diagram.](https://learn.microsoft.com/en-us/purview/media/dspm-workflow.png)
1. **Opt-in to analytics processing**: To get started with DSPM (preview), you must enable and opt in to:
    1. Insider risk management analytics
    2. DLP analytics
    3. Analytics processing in DSPM (preview) to scan for unprotected data in your organization.
2. **Evaluate insights and take action**: After the automated analytics processing is completed, you can evaluate the insights created by DSPM (preview) to help mitigate risks for unprotected data.
3. **Actions**:
    1. **Investigate with Security Copilot**: Use built-in and custom prompts with Security Copilot to help identify specific areas of risk.
    2. **Create policies with recommendations**: Use recommendations to quickly create insider risk management and DLP policies to help mitigate data security risks for unprotected data assets.
4. **Track posture with analytic trends and reports**: Use analytic trends and reports to view your posture over time and for data locations across your organization.