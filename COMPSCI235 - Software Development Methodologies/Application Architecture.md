![[Pasted image 20231101235727.png]]
- Each module has a well-defined responsibility ([[Single Responsibility Principle (SRP)]])
- Request handlers (views) are concerned with:
	- extracting information from [[Hypertext Transfer Protocol (HTTP)]] requests
	- creating [[Hypertext Markup Language (HTML)]]
- The service layer is responsible for:
	- fetching data from the repository
	- processing requests using the data
	- updating repository data
		- FORM, login...

![[Pasted image 20231102000143.png]]