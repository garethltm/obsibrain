a simple framework that simplifies working with [[Hypertext Markup Language (HTML)]] forms
- When using [[WTForms]], an additional environment variable must be supplied in the `.env` file & loaded at application startup
		- `WTF_CSRF_SECRET_KEY` - if not set up, it would use Default SECRET_KEY value
		- [[WTForms]] uses the value for `WTF_CSRF_SECRET_KEY` when creating a [[csrf]]
### Key concepts provided by [[WTForms]]:
![[Pasted image 20231102100746.png]]
- Forms
- Field
	- String, Date/Time field
- Validators
	- Length should be, ..., 