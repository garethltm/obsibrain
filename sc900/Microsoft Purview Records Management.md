Organizations of all types require a management solution to manage regulatory, legal, and business-critical records across their corporate data. 

[[Microsoft Purview Records Management]] helps an organization look after their legal obligations. It also helps to demonstrate compliance with regulations, and increases efficiency with regular disposition of items that are no longer required to be kept, no longer of value, or no longer required for business purposes. [[Microsoft Purview Records Management]] includes many features, including:
- Labeling content as a record.
- Establishing retention and deletion policies within the record label.
- Triggering event-based retention.
- Reviewing and validating disposition.
- Proof of records deletion.
- Exporting information about disposed items.

When content is labeled as a record, by using a retention label, the following happens:
- Restrictions are put in place to block certain activities.
- Activities are logged.
- Proof of disposition is kept at the end of the retention period.

To enable items to be marked as records, an administrator sets up retention labels.![An admin can choose for items to be marked as records when configuring a policy.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-purview-risk-compliance-governance/media/mark-items-record.png)
Items such as documents and emails can then be marked as records based on those retention labels. Items might be marked as records, but they can also be shown as regulatory records. Regulatory records provide other controls and restrictions such as:
- A regulatory label can’t be removed when an item has been marked as a regulatory record.
- The retention periods can’t be made shorter after the label has been applied.

The most important difference is that if content has been marked as a regulatory record, nobody, not even a global administrator, can remove the label. Marking an item as a regulatory record can have irreversible consequences, and should only be used when necessary. As a result, this option isn’t available by default, and has to be enabled by the administrator using PowerShell.
### Common use cases
There are different ways in which [[Microsoft Purview Records Management]] can be used across an organization, including:
- Enabling administrators and users to manually apply retention and deletion actions for documents and emails.
- Automatically applying retention and deletion actions to documents and emails.
- Enabling site admins to set default retain and delete actions for all content in a SharePoint library, folder, or document set.
- Enabling users to automatically apply retain and delete actions to emails by using Outlook rules.

To ensure [[Microsoft Purview Records Management]] is used correctly across the organization, administrators can work with content creators to put together training materials. Documentation should explain how to apply labels to drive usage, and ensure a consistent understanding.