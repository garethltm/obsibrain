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
Data loss can harm an organization’s customers, business processes, and the organization itself. Organizations need to prevent data loss by detecting risky behavior and preventing sensitive information from being shared inappropriately.

In [[Microsoft Purview]], you implement data loss prevention (DLP) by defining and applying DLP policies. With a DLP policy, you can **identify, monitor, and automatically protect** sensitive items across:
- Microsoft 365 services such as Teams, Exchange, SharePoint, and OneDrive accounts
- Office applications such as Word, Excel, and PowerPoint
- Windows 10, Windows 11, and macOS (three latest released versions) endpoints
- Cloud apps
- On-premises file shares and on-premises SharePoint
- Power BI

DLP detects sensitive items by using deep content analysis, not by just a simple text scan. Content is analyzed for primary data matches to keywords, by the evaluation of regular expressions, by internal function validation, and by secondary data matches that are in proximity to the primary data match. Beyond that DLP also uses [[Machine Learning (ML)]] algorithms and other methods to detect content that matches your DLP policies.
## Protective actions of DLP policies
DLP policies are how you monitor the activities that users take on sensitive items at rest, sensitive items in transit, or sensitive items in use and take protective actions. Protective actions that DLP policies can take include:
- Show a pop-up policy tip to the user that warns them that they may be trying to share a sensitive item inappropriately.
- Block the sharing and, via a policy tip, allow the user to override the block and capture the users' justification.
- Block the sharing without the override option.
- For data at rest, sensitive items can be locked and moved to a secure quarantine location,
- For Teams chat, the sensitive information won't be displayed.

All DLP monitored activities are recorded to the Microsoft 365 Audit log by default and routed to Activity explorer. When a user performs an action that meets the criteria of a DLP policy, and you have alerts configured, DLP provides alerts in the DLP alert management dashboard.
## DLP Policy information
![A screen capture of the landing page when creating a DLP policy. The screen shows the option of starting with a template or custom policy.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/data-loss-prevention-policy-create-v2.png)
![A screen capture from creating a DLP policy. The screen shows the options for choosing a location to apply a DLP policy.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/data-loss-prevention-policy-locations-v2.png)
DLP policies can be created from predefined templates, or you can create a custom policy. No matter which you choose, all DLP policies require the same information.

- Choose the type of data to monitor. Predefined policy templates allow you to choose from categories such as Financial data, Medical and health data, or Privacy data for various countries and regions. Alternatively, you can create a custom policy that uses the available sensitive information types, retention labels, and sensitivity labels.
- Choose administrative scoping. DLP policies can be applied to all users and groups by an unrestricted administrator, or they can be scoped to administrative units. Administrative units let you subdivide your organization into smaller units, and then assign specific administrators that can manage only the members of those units.
- Choose the location where the policy will be applied, such as Exchange, SharePoint, OneDrive, and more.
- Choose the conditions that must be matched for a policy to be applied to an item.
- Choose the protective action to take when the policy conditions are met.
## Endpoint data loss prevention
![A screenshot of data classification information in the activity explorer as monitored through endpoint DLP.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/data-loss-prevention-activity-explorer.png)
Endpoint DLP enables you to audit and manage the many activities users take on sensitive items that are physically stored Windows 10, Windows 11, or macOS devices. The list that follows shows a few examples:
- Creating an item
- Renaming an item
- Copying items to removable media
- Copying items to network shares
- Printing documents
- Accessing items using unallowed apps and browsers

In the activity explorer, you can view information about what users are doing with sensitive content.
## Data loss prevention in Microsoft Teams
![A screenshot of a Microsoft Teams chat that was blocked that includes a link for the user to obtain more information.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/5-data-loss-prevention-policy-tip-v2.png)
Data loss prevention capabilities extend to Microsoft Teams chat and channel messages, whether it's in a message or a file, including messages in private channels. Just like with Exchange, Outlook, SharePoint, and OneDrive, administrators can use DLP policy tips that will be displayed to the user to show them why a policy has been triggered. For example, the screenshot that follows shows a policy tip on a chat message that was blocked because the user attempted to share a U.S. Social Security Number.
>User can then find out more about why their message was blocked by selecting the "What can I do?" link, and take appropriate action.![A screenshot of a DLP policy tip presented to user whose message is blocked. The tip provides information about why their message was blocked, and actions to take.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/5-policy-tip-more-information.png)
	DLP policies applied to Microsoft 365 services, including Microsoft Teams, can help users across organizations to collaborate securely and in a way that's in line with compliance requirements.
## Integration with [[Microsoft Security Copilot]]
![Screen capture of the Microsoft Purview capabilities available Microsoft Security Copilot.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/purview-capabilities.png)
[[Microsoft Purview]] Data Loss Prevention supports integration with [[Microsoft Security Copilot]], through the standalone and embedded experiences.

To experience this Copilot capability, organizations must be onboarded to Copilot, have enabled Copilot to access data from Microsoft 365 services, and users must have the appropriate role permissions,

The Microsoft Purview capabilities, that you can view in the standalone experience by selecting the prompt icon and selecting all capabilities, are built-in prompts that you can use but you can also enter your own prompts based on the capabilities supported.

![Screen capture of a data loss prevention alert page that shows the option to summarize the alert.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/copilot-alert.png)![Screen capture of a data loss prevention alert summary generated by Copilot.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/copilot-alert-summary.png)
In the embedded experience, [[Microsoft Security Copilot]] in [[Microsoft Purview]] Data Loss Prevention supports alert summarization. To access Copilot from within [[Microsoft Purview]] Data Loss Prevention, navigate to the alerts queue to select the alert you want to review. Information about the alert and the option to summarize the alert are displayed. You select Summarize to have Copilot generate the alert summary.
## Insider Risk Management
[[Microsoft Purview]] Insider Risk Management is a solution that helps minimize internal risks by enabling an organization to detect, investigate, and act on risky and malicious activities.

Managing and minimizing risk in an organization starts with understanding the types of risks found in the modern workplace. Some risks are driven by external events and factors, and are outside an organization’s direct control. Other risks are driven by internal events and employee activities that can be eliminated and avoided. 
>Some examples include:
>- Leaks of sensitive data and data spillage
>- Confidentiality violations
>- Intellectual property (IP) theft
>- Fraud
>- Insider trading
>- Regulatory compliance violations

Insider risk management is centered around the following principles:
- **Transparency**: Balance user privacy versus organization risk with privacy-by-design architecture.
- **Configurable**: Configurable policies based on industry, geographical, and business groups.
- **Integrated**: Integrated workflow across Microsoft Purview solutions.
- **Actionable**: Provides insights to enable user notifications, data investigations, and user investigations.
## Insider risk management workflow
![A diagram of the insider risk management workflow.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/insider-risk-management-workflow.png)
Insider risk management helps organizations to identify, investigate, and address internal risks. With focused policy templates, comprehensive activity signaling across Microsoft 365, and a flexible workflow, organizations can take advantage of actionable insights to help identify and resolve risky behavior quickly. Identifying and resolving internal risk activities and compliance issues with insider risk management in Microsoft Purview is achieved using the following workflow:
