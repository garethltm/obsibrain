- enables organizations to efficiently manage group memberships, access to enterprise applications & role assignment. 
	- Regular [[Access Reviews]] ensure that only the right people have access to resources. 
	- Excessive access rights are a known security risk.

[[Microsoft Entra ID]] enables you to collaborate with users from inside your organization & with external users. Users can join groups, invite guests, connect to cloud apps & work remotely from their work or personal devices. This convenience has led to a need for better access management capabilities.
## Use Cases
1. Too many users in privileged roles
	- It's a good idea to check how many users have administrative access & if there are any invited guests or partners that haven't been removed after being assigned to do an administrative task. You can recertify the role assignment of users in Microsoft Entra roles such as Global Administrators, or Azure resources roles such as User Access Administrator in the Microsoft [[Privileged Identity Management (PIM)]] experience.
2. Business critical data access
	- For certain resources, such as business critical applications , it might be required as part of compliance processes to ask people to regularly reconfirm & give a justification on why they need continued access
3. To maintain a policy's exception list
	- Sometimes there are business cases that require you to make exceptions to policies. As the IT admin, you can manage this task & provide auditors with proof that these exceptions are reviewed regularly
4. Ask group owners to confirm they still need guests in their groups
	- If a group gives guests access to business sensitive content, then it's the group owner's responsibility to confirm the guests still have a legitimate business need for access.
5. Have reviews recur periodically
	- You can set up recurring access reviews of users at set frequencies such as weekly, monthly, quarterly or annually. Reviewers are notified at the start of each review & upon completion approve or deny access through a friendly user interface & with the help of smart recommendations
### Multi-stage access reviews
- Microsoft Entra [[Access Reviews]] support up to 3 review stages, in which multiple types of reviewers engage in determining who still needs access to company resources.
- Multi-stage access reviews allow you & your organization to enable complex workflows to meet recertification & audit requirements calling for multiple reviewers to attest to access for users in particular sequence. It also helps you design more efficient reviews for your resource owners & auditors by reducing the number of decisions each reviewer is accountable for.![Screen capture of an access review notification that invites users to review access rights.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-identity-protection-governance-capabilities/media/3-access-reviews-invite-users-to-review-access-rights.png)
