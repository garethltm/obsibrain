Sensitive information types (SIT) are pattern-based classifiers. They have set patterns that can be used to identify them. 
>For example, an identification number in a country/region may be based on a specific pattern, like this:
>
>_123-456-789-ABC_

[[Microsoft Purview]] includes many built-in sensitive information types based on patterns that are defined by a regular expression (regex) or a function.
>Examples include:
>- Credit card numbers
>- Passport or identification numbers
>- Bank account numbers
>- Health service numbers

Data classification in [[Microsoft Purview]] also supports the ability to create custom sensitive information types to address organization-specific requirements. 
>For example, an organization may need to create sensitive information types to represent employee IDs or project numbers.

Also supported is exact data match (EDM) classification. EDM-based classification enables you to create custom sensitive information types that refer to exact values in a database of sensitive information. In the [[Microsoft Purview]] portal sensitive information types are referred to as **EDM classifiers**.

Sensitive information types can be used with sensitivity labels, retention labels, and across many Microsoft Purview and Microsoft Priva Solutions.