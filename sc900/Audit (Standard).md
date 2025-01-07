is turned on by default for all organizations with the appropriate subscription and available to users with the appropriate permissions. When an audited activity is performed by a user or admin, an audit record is generated and stored in the audit log for your organization. In Audit (Standard), records are retained for 180 days. You can retrieve audit logs that occur in most of the Microsoft 365 services in your organization by using the following methods:
- The audit log search tool in the Microsoft Purview portal.
- The Office 365 Management Activity API
- The `Search-UnifiedAuditLog` cmdlet in Exchange Online PowerShell

After you search the audit log, you can export the audit records returned by the search, to a CSV file, enabling further analysis using Microsoft Excel or Excel Power Query.