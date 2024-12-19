[[Microsoft Entra ID]] Protection helps organizations detect, investigate, and remediate identity-based risks. These identity-based risks can be further fed into tools like [[Conditional Access]] to make access decisions or fed back to a [[security information and event management (SIEM)]] tool for further investigation and correlation.

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
	- A risky sign-in is reported when there are one or more 
- Risky users: