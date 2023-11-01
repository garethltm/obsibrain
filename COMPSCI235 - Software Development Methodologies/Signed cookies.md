#### Application vulnerability
![[Pasted image 20231102011313.png]]

### How to resolve the vulnerability
##### Signed cookies
![[Pasted image 20231102011452.png]]

[[Signed cookies]] in [[Flask]]
- [[Flask]] provides support for [[Signed cookies]] via the session global object
	- session essentially presents like **dictionary**; the state is held in a cookie is represented by key/value pairs
	- the secret is supplied by the application in an environment variable named `SECRET_KEY` which can be found in the `.env` file
![[Pasted image 20231102011820.png]]

Related to: [[Authentication]], [[cookie]]