
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