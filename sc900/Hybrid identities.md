Because organizations are moving workload to the cloud, but many still use a mix of on-premise and cloud applications $\rightarrow$ users need easy access to applications regardless of where they are hosted, which requires a single identity across these applications.

Microsoft's identity solutions provide this by creating a common identity for [[sc900/Authentication|Authentication]] and [[Authorization]], known as hybrid identity. This achieved through provisioning and synchronization:
1. Provisioning: Creating an identity between different directory services, such as provisioning a user from Azure [[Active Directory (AD)]] to [[Microsoft Entra ID]].
2. Synchronization: Ensuring that identity information for on-premise users and groups matches the cloud
