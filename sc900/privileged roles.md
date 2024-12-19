[[Microsoft Entra ID]] has roles and permissions that are identified as privileged. These roles and permissions can be used to delegate management of directory resources to other users, modify credentials, [[authentication]] or [[authorization]] policies, or access restricted data. Privileged role assignments can lead to elevation of privilege if not used in a secure and intended manner.![Screenshot of the Microsoft Entra roles and administrators page that shows the Privileged and Assignments columns.](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/media/privileged-roles-permissions/privileged-roles-portal.png)

[Built-in roles available](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference)
### Application Administrator
![Screenshot of the Microsoft Entra roles and administrators page that shows the privileged permissions for a role.](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/media/privileged-roles-permissions/privileged-roles-permissions.png)
### Custom Role
![Screenshot of the New custom role page that shows a custom role with privileged permissions.](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/media/privileged-roles-permissions/custom-role-privileged-permissions.png)
## Best practices
- Apply principle of least privilege
- Use [[Privileged Identity Management (PIM)]] to grant just-in-time access
- Turn on multi-factor authentication for all your administrator accounts
- Configure recurring access reviews to revoke unneeded permissions over time
- Limit the number of Global Administrators to less than 5
- Limit the number of privileged role assignments to less than 10

![[Pasted image 20241219142611.png]]

See more: ![https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/privileged-roles-permissions?tabs=admin-center]