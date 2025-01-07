reduces risk and complexity with unified data security, governance, and compliance solutions for the era of AI.
### Understand & explore the data
![A screenshot of the activity explorer page in the Microsoft Purview portal.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/activity-explorer.png)![A screenshot of the content explorer page in the Microsoft Purview portal.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/content-explorer.png)
Data classification can involve large numbers of documents and emails. To help administrators derive insights and understanding, the Explorers node under Information Protection in the [[Microsoft Purview]] portal provides tools such as the activity explorer and content explorer that provide details at a glance, including:
- The number of items classified as sensitive information and which classifications they are.
- Details on the locations of data based on sensitivity.
- Summary of actions that users are taking on sensitive content across the organization.

Administrators can also use the information gained from these tools to guide their actions.
- _**Content explorer**_: 
	- Content explorer provides a current snapshot of the items that have a sensitivity label, a retention label or have been classified as a sensitive information type in your organization. It enables administrators with the appropriate role permissions to further drill down into items by allowing them to access and review the scanned source content that's stored in different kinds of locations, such as Exchange, SharePoint, and OneDrive.
	- Access to content explorer is highly restricted because it makes it possible to read the contents of scanned files. A user that requires access to content explorer must have an account in one or more of the content explorer roles groups.
    
- _**Activity explorer**_: 
	- Activity explorer provides visibility into what content has been discovered and labeled, and where that content is. It makes it possible to monitor what's being done with labeled content across the organization. Admins gain visibility into document-level activities like label changes and downgrades (such as when someone changes a label from confidential to public), or when files are copied to removable media or a network share.
	- Admins use the filters to see all the details for a specific label, including file types, users, and activities. Activity explorer helps you understand what's being done with labeled content over time. Admins use activity explorer to evaluate if controls already in place are effective.
## Sensitivity labels
![A screen capture of a sensitivity label named Confidential-Finance, which includes settings for encryption, content marking, and autolabeling for files and emails.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/sensitivity-label-v2-inline.png)
Sensitivity labels enable the labeling and protection of content, without affecting productivity and collaboration. With sensitivity labels, organizations can decide on labels to apply to content such as emails and documents, much like different stamps are applied to physical documents:

Labels are:
- **Customizable**: Admins can create different categories specific to the organization, such as Personal, Public, Confidential, and Highly Confidential.
- **Clear text**: Because each label is stored in clear text in the content's metadata, third-party apps and services can read it and then apply their own protective actions, if necessary.
- **Persistent**. After you apply a sensitivity label to content, the label is stored in the metadata of that email or document. The label then moves with the content, including the protection settings, and this data becomes the basis for applying and enforcing policies.

Each item that supports sensitivity labels can only have one label applied to it, at any given time.

Sensitivity labels can be configured to:
- **Encrypt** email only or both email and documents.
- **Mark the content** when Office apps are used. Marking the content includes adding watermarks, headers, or footers. Headers or footers can be added to emails or documents. Watermarks can be applied to documents but not to email.
- **Apply the label automatically** in Office apps or recommend a label. Admins choose the types of sensitive information to be labeled. The label can be applied automatically or configured to prompt users to apply the recommended label.
- **Protect content in containers such as sites and groups**. This label configuration doesn't result in documents being automatically labeled. Instead, the label settings protect content by controlling access to the container where documents are stored.
- **Extend sensitivity labels to third-party apps and services**. The Microsoft Purview Information Protection SDK enables third-party apps to read sensitivity labels and apply protection settings.
- **Classify content without using any protection settings**. A classification can be assigned to content (just like a sticker) that persists and roams with the content as it's used and shared. The classification can be used to generate usage reports and view activity data for sensitive content.

The image that follows shows the settings for a sensitivity label named Confidential-Finance, which includes settings for encryption, content marking, and autolabeling for files and emails.
## Label policies
After sensitivity labels are created, they need to be published to make them available to people and services in the organization. Sensitivity labels are published to users or groups through label policies. Sensitivity labels will then appear in Office apps for those users and groups. The sensitivity labels can be applied to documents and emails. Label policies enable admins to:

- **Choose the users and groups that can see labels**. Labels can be published to specific users, distribution groups, Microsoft 365 groups in Microsoft Entra ID, and more.
- **Apply a default label** to all new emails and documents that the specified users and groups create. Users can always change the default label if they believe the document or email has been mislabeled.
- **Require justifications for label changes**. If a user wants to remove a label or replace it, admins can require the user to provide a valid justification to complete the action. The user will be prompted to provide an explanation for why the label should be changed.
- **Require users to apply a label (mandatory labeling)**. It ensures a label is applied before users can save their documents, send emails, or create new sites or groups.
- **Link users to custom help pages**. It helps users to understand what the different labels mean and how they should be used.

Once a sensitivity label is applied to an email or document, any configured protection settings for that label are enforced on the content.
## Data loss prevention (DLP)

## Integration with [[Microsoft Security Copilot]]
![Screen capture of the Microsoft Purview capabilities available Microsoft Security Copilot.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/purview-capabilities.png)
[[Microsoft Purview Insider Risk Management]] supports integration with [[Microsoft Security Copilot]], through the standalone and embedded experiences.

To experience Copilot integration, organizations must be onboarded to Copilot, have enabled Copilot to access data from Microsoft 365 services, and users must have the appropriate role permissions.

The [[Microsoft Purview]] capabilities, that you can view in the standalone experience by selecting the prompt icon and selecting all capabilities, are built-in prompts that you can use, but you can also enter your own prompts based on the capabilities supported.

![Screen capture of an Insider Risk Management alerts page that shows the option to summarize an alert.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/copilot-risk-management.png)![Screen capture of an Insider Risk Management alert summary generated by Copilot.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/copilot-risk-management-summary.png)
In the embedded experience, Copilot in Microsoft Purview Insider Risk Management supports alert summarization. To access Copilot from within Microsoft Purview Insider Risk Management, navigate to the alerts queue to select the alert you want to review. Information about the alert and the option to summarize the alert are displayed. You select Summarize to have Copilot generate the alert summary.
## Adaptive Protection
Adaptive protection in Microsoft Purview uses machine learning (ML) to identify the most critical risks and proactively and dynamically apply protection controls from:

- Data Loss Prevention
- Microsoft Purview Data Lifecycle Management (preview)
- Microsoft Entra Conditional Access (preview)

Integration with data loss prevention, data lifecycle management, and Conditional Access can help organizations automate their response to insider risks and reduce the time required to identify and remediate potential threats. By using the capabilities of all four solutions, organizations can create a more comprehensive security framework that addresses both internal and external threats.

Adaptive protection helps mitigate potential risks by using:

- Context-aware detection. Helps identify the most critical risks with ML-driven analysis of both content and user activities.
- Dynamic controls. Helps enforce effective controls on high-risk users while others maintain productivity.
- Automated mitigation. Helps to minimize the impact of potential data security incidents and reduce admin overhead.

Adaptive protection dynamically assigns appropriate data loss prevention, data lifecycle management, and Conditional Access policies to users based on the insider risk levels (elevated, moderate, or minor) defined and analyzed by the machine learning models in Insider Risk Management. Policies become adaptive based on user context, ensuring that the most effective policy, such as blocking data sharing through data loss prevention or blocking application access through Conditional Access, is applied only to high-risk users while low-risk users maintain productivity.