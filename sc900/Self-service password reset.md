Self-service password reset (SSPR) in Microsoft Entra ID is indeed a powerful feature! It offers several benefits:

1. **Cost Reduction**: By allowing users to reset their passwords independently, it significantly reduces IT support costs.
2. **Increased Productivity**: Users can quickly get back to work without waiting for help desk assistance.
3. **Flexible Security**: Administrators can update security settings and roll them out without disrupting user sign-ins.
4. **Robust Auditing**: SSPR provides detailed audit logs that can be integrated into a Security Incident and Event Monitoring (SIEM) system.

To use SSPR, users need to:

- Have a Microsoft Entra ID license.
- Be enabled for SSPR by an administrator.
- Register their authentication methods (at least two are recommended).

Available authentication methods include:

- Mobile app notification
- Mobile app code
- Email
- Mobile phone
- Office phone
- Security questions (not available for administrator accounts)

When registering, users choose their preferred methods. Security questions are used only during the SSPR process as a secondary form of authentication.