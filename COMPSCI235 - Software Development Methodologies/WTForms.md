a simple framework that simplifies working with [[Hypertext Markup Language (HTML)]] forms
- When using [[WTForms]], an additional environment variable must be supplied in the `.env` file & loaded at application startup
		- `WTF_CSRF_SECRET_KEY` - if not set up, it would use Default SECRET_KEY value
		- [[WTForms]] uses the value for `WTF_CSRF_SECRET_KEY` when creating a [[Cross-site Request Forgery (CSRF)]] token
- When testing a Web app that uses [[WTForms]], configuration variable named `WTF_CSRF_ENABLED` should be set to False
	- The [[Flask]] client doesn't process or relay [[Cross-site Request Forgery (CSRF)]] tokens
### Key concepts provided by [[WTForms]]:
![[Pasted image 20231102100746.png]]
- Forms
- Field
	- String, Date/Time field
- Validators
	- Length should be, ..., 