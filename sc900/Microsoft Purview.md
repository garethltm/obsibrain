
### Understand & explore the data
![A screenshot of the activity explorer page in the Microsoft Purview portal.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/activity-explorer.png)![A screenshot of the content explorer page in the Microsoft Purview portal.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-data-solutions/media/content-explorer.png)
Data classification can involve large numbers of documents and emails. To help administrators derive insights and understanding, the Explorers node under Information Protection in the [[Microsoft Purview]] portal provides tools such as the activity explorer and content explorer that provide details at a glance, including:
- The number of items classified as sensitive information and which classifications they are.
- Details on the locations of data based on sensitivity.
- Summary of actions that users are taking on sensitive content across the organization.

Administrators can also use the information gained from these tools to guide their actions.
- _**Content explorer**_: 
	- Content explorer provides a current snapshot of the items that have a sensitivity label, a retention label or have been classified as a sensitive information type in your organization. It enables administrators with the appropriate role permissions to further drill down into items by allowing them to access and review the scanned source content that's stored in different kinds of locations, such as Exchange, SharePoint, and OneDrive.
    
    Access to content explorer is highly restricted because it makes it possible to read the contents of scanned files. A user that requires access to content explorer must have an account in one or more of the content explorer roles groups.
    
- _**Activity explorer**_: Activity explorer provides visibility into what content has been discovered and labeled, and where that content is. It makes it possible to monitor what's being done with labeled content across the organization. Admins gain visibility into document-level activities like label changes and downgrades (such as when someone changes a label from confidential to public), or when files are copied to removable media or a network share.
    
    Admins use the filters to see all the details for a specific label, including file types, users, and activities. Activity explorer helps you understand what's being done with labeled content over time. Admins use activity explorer to evaluate if controls already in place are effective.