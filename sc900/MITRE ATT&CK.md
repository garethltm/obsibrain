is a curated [[Knowledge Base (KB)]] that tracks cyber adversary tactics and techniques used by [threat actors](https://www.crowdstrike.com/en-us/cybersecurity-101/threat-intelligence/threat-actor/) across the entire attack lifecycle. The framework is meant to be more than a collection of data: it is intended to be used as a tool to strengthen an organization’s security posture.

For instance, because [[MITRE ATT&CK]] takes the perspective of the adversary, security operations teams can more easily deduce an adversary’s motivation for individual actions and understand how those actions relate to specific classes of defenses.
### Where does the data in the MITRE ATTACK Framework come from?
[[MITRE ATT&CK]] is populated mainly by publicly available threat intelligence and incident reporting, as well as by research on new techniques contributed by cyber security analysts and threat hunters. It is used by those same professionals to better understand the different ways bad actors might operate so adversarial behavior can be detected and stopped.
### Tactics
Adversarial tactics are specific technical objectives that an adversary intends to achieve. Tactics are categorized according to these objectives. For instance, there are currently [14 tactics](https://attack.mitre.org/tactics/enterprise/) cataloged in the enterprise matrix:
- **Reconnaissance**: Techniques that actively or passively gather information to plan future targeted attacks.
- **Resource development**: Involves attackers purchasing or stealing resources to use them for a future attack.
- **Initial access**: Techniques where adversaries try to gain a foothold in your network through different attack vectors.
- **Execution**: Adversary techniques that try to run malicious code on a local or remote system.
- **[Persistence](https://www.crowdstrike.com/en-us/cybersecurity-101/threat-intelligence/advanced-persistent-threat-apt/)**: Tactics that involve adversaries trying to maintain their foothold in your local or remote network.
- [**Privilege escalation**](https://www.crowdstrike.com/en-us/cybersecurity-101/cyberattacks/privilege-escalation/): When an adversary tries to gain higher-level permission into your organization’s network.
- **Defense evasion**: Adversary techniques to avoid detection when they move through your network.
- **Credential access**: Tactics focused on retrieving sensitive credentials such as passwords.
- **Discovery**: When adversaries try to gain an understanding of how your systems work.
- **[Lateral movement](https://www.crowdstrike.com/en-us/cybersecurity-101/cyberattacks/lateral-movement/)**: Involves adversaries that enter and control systems, moving through your network.
- **Collection**: Techniques that gather information from relevant sources within your organization.
- **Command and Control ([C2 or C&C](https://www.crowdstrike.com/en-us/cybersecurity-101/cyberattacks/command-and-control-cac-attack/))**: When adversaries communicate with compromised systems to gain control.
- [**Exfiltration**](https://www.crowdstrike.com/en-us/cybersecurity-101/cyberattacks/data-exfiltration/): Consists of techniques that straight up steal data from your network.
- **Impact**: When adversaries focus on disrupting data availability or integrity and interrupting business operations.
### Techniques
**A technique describes one specific way an adversary may try to achieve an objective**. A multitude of techniques are documented under each “tactics” category. This is because adversaries may use different techniques depending on factors such as their skills sets, targets’ system configuration aned availability of suitable tools.

Each technique includes a description of the method, the systems and platforms it pertains to, which adversary groups use it (if that is known), ways to mitigate the activity, and references to its use in the real world.

MITRE ATT&CK currently identifies [188 techniques and 379 sub-techniques for enterprise](https://attack.mitre.org/techniques/enterprise/).