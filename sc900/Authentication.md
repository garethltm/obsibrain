- the process of proving that a person is who they say they are

## Phone
Microsoft Entra ID offers two options for phone-based [[authentication]]:
1. **SMS-based [[Authentication]]**:
    - **Primary Authentication**: Users can sign in using their mobile phone number and a verification code sent via SMS, without needing a username and password.
    - **Secondary Authentication**: Used during self-service password reset (SSPR) or multifactor authentication (MFA), where a verification code is sent via SMS to supplement the password.
2. **Voice Call Verification**:
    - **Secondary Authentication**: Used during SSPR or MFA, where an automated voice call prompts the user to press # on their keypad to verify their identity. Voice calls are not supported as a primary form of authentication.

## OATH
OATH (Open Authentication) is an open standard for generating time-based, one-time password (TOTP) codes used for user authentication.
- Software OATH Tokens: Applications that generate OTPs using a secret key (seed) provided by Microsoft Entra ID.
- Hardware OATH Tokens: Small devices (like key fobs) that display a code refreshing every 30 or 60 seconds, with a preprogrammed secret key.
Both software and hardware OATH tokens are used as secondary forms of authentication in Microsoft Entra ID, particularly for self-service password reset (SSPR) or multifactor authentication (MFA).

## Passwordless authentication
The end-goal for many organizations is to remove the use of passwords as part of sign-in events. When a user signs in with a passwordless method, credentials are provided by using methods like biometrics with Windows Hello for Business, or a FIDO2 security key. These authentication methods can't be easily duplicated by an attacker.

[[Microsoft Entra ID]] provides ways to natively authenticate using passwordless methods to simplify the sign-in experience for users and reduce the risk of attacks.

The following video explains the problem with passwords, and why passwordless authentication is so important.

