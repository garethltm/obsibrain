- helps organizations detect, investigate, and remediate identity-based risks. These identity-based risks can be further fed into tools like [[conditional access]] to make access decisions or fed back to a [[security information and event management (SIEM)]] tool for further investigation and correlation.

![[Pasted image 20241219131616.png]]
### Detect risks
- Detect risky behaviors like:
	- Anonymous IP address usage
	- Password spray attacks
	- Leaked credentials
	- and more...
	During each sign-in, ID Protection runs all real-time sign-in detections generating a sign-in session risk level, indicating how likely the sign-in is compromised. Based on this risk level, policies are then applied to protect the user and the organization.
### Investigate risks
- Risk detections:
	- Each risk detected is reported as a risk detection
- Risky sign-ins:
	- A risky sign-in is reported when there are one or more risk detections reported for that sign-in
- Risky users:
	- A Risky user is reported when either or both are true:
		1. The user has one or more Risky sign-ins
		2. One or more risk detections are reported
### Remediate risks
1. Automatic remediation
	- Risk-based [[conditional access]] policies an be enabled to require access controls such as providing a strong authentication method, perform multifactor authentication, or perform a secure password reset based on the detected risk level. If the user successfully completes the access control, the risk is automatically remediated.
2. Manual remediation
	- When user remediation isn't enabled, an administrator must manually review them in the reports in the portal, through the API, or in Microsoft 365 Defender. Administrators can perform manual actions to dismiss, confirm safe, or confirm compromise on the risks.
### Making use of the data
Data from ID Protection can be exported to other tools for archive, further investigation, and correlation. The Microsoft Graph based APIs allow organizations to collect this data for further processing in a tool such as their [[Security Information and Event Management (SIEM)]].

Organizations might store data for longer periods by changing the diagnostic settings in [[Microsoft Entra ID]]. They can choose to send data to a Log Analytics workspace, archive data to a storage account, stream data to Event Hubs, or send data to another solution.
## Required roles
![[Pasted image 20241219141303.png]]
## License requirements
![[Pasted image 20241219141328.png]]