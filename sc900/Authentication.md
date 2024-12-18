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

## Windows Hello for Business
Windows Hello for Business replaces passwords with strong two-factor authentication on devices. This involves a combination of a key or certificate tied to a device and either a PIN or biometrics. Both PIN entry and biometric gestures trigger the use of a private key to sign data cryptographically, which is then verified by the [[identity provider]].

This method helps protect against credential theft, as an attacker would need both the device and the biometric info or PIN. Windows Hello for Business can be used as a primary form of passwordless authentication and as a secondary form of authentication during multifactor authentication (MFA).

## FIDO2
Fast Identity Online (FIDO) is an open standard for passwordless authentication, allowing users to sign in using an external security key or a built-in platform key, eliminating the need for usernames and passwords.

FIDO2 is the latest standard, incorporating WebAuthn, and is supported by Microsoft Entra ID. FIDO2 security keys are unphishable and can come in various forms, such as USB, Bluetooth, or NFC devices. These keys enhance security by eliminating passwords that could be exposed or guessed.

Users can sign in to [[Microsoft Entra ID]], hybrid joined Windows 10 devices, and supported browsers using FIDO2 security keys, providing single sign-on to cloud and on-premises resources. FIDO2 is ideal for security-sensitive enterprises or users who prefer not to use their phone as a second factor. It serves as both a primary and secondary form of authentication during multifactor authentication (MFA).
## Microsoft Authenticator
As a passwordless authentication method, the Microsoft Authenticator app can be used as a primary form of authentication to sign in to any Microsoft Entra account or as an additional verification option during self-service password reset (SSPR) or Microsoft Entra multifactor authentication events.

To use Microsoft Authenticator, a user must download the phone app from the Microsoft store and register their account. Microsoft Authenticator is available for Android and iOS.

With Passwordless sign-in, the Authenticator App turns any iOS or Android phone into a strong, passwordless credential. To sign in to their Microsoft Entra account, a user enters their username, matches a number displayed on the screen to the one on their phone, then uses their biometric or PIN to confirm.