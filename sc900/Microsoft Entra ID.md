- Microsoft's cloud-based [[Identity and Access Management (IAM)]] service (used to be called Azure Active Directory)
- simplifies the way organizations manage [[Authorization]] and access by providing a single [[Identity]] system for their cloud and on-premises applications. [[Microsoft Entra ID]] can be synchronized with your existing on-premise [[Active Directory (AD)]], synchronized with other directory services, or used as a standalone service.

[[Microsoft Entra ID]] also allows organizations to securely enable the use of personal devices![Diagram showing Microsoft Entra ID as a cloud-based identity provider that works with cloud apps such as M365, devices, and on-premises applications.](https://learn.microsoft.com/en-us/training/wwl-sci/explore-basic-services-identity-types/media/entra-id-general-diagram-v2.png)

## Identity Secure Score
- a percentage that functions as an indicator for how aligned you are with Microsoft's best practice recommendations for security. Each improvement action in identity secure score is tailored to your specific configuration

## Manage devices in Microsoft Entra ID
- provides a central place to manage device identities & monitor related event information![Screenshot that shows the devices overview.](https://learn.microsoft.com/en-us/entra/identity/devices/media/manage-device-identities/devices-azure-portal.png)

### Manage an Intune device
- Enable/disable a Microsoft Entra device
- Delete a Microsoft Entra device
- View/copy a device ID
- View/copy BitLocker keys![Screenshot that shows how to view BitLocker keys.](https://learn.microsoft.com/en-us/entra/identity/devices/media/manage-device-identities/show-bitlocker-key.png)
	- To view or copy BitLocker keys, you need to be the owner of the device or have one of these roles:
		- Cloud Device Administrator
		- Helpdesk Administrator
		- Intune Administrator
		- Security Administrator
		- Security Reader
- View/filter your devices
- Download devices
- Configure device settings
	- they need to be either registered or joined to [[Microsoft Entra ID]]
	- You must be assigned one of the following roles to read or modify device settings:
		- [Cloud Device Administrator](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference#cloud-device-administrator) (read and modify)
		- [Intune Administrator](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference#intune-administrator) (read only)
		- [Windows 365 Administrator](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference#windows-365-administrator) (read only)![Screenshot that shows device settings related to Microsoft Entra ID.](https://learn.microsoft.com/en-us/entra/identity/devices/media/manage-device-identities/device-settings-azure-portal.png)
[Manage devices in Microsoft Entra ID](https://learn.microsoft.com/en-us/entra/identity/devices/manage-device-identities)