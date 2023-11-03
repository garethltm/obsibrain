splitting services into smaller modules
>	#Example 
>	they can interact with each other using messages

![[Pasted image 20231104013117.png]]

An approach to developing a single application as a suite of small services, each running its own process & communicating with lightweight mechanisms, often an [[Hypertext Transfer Protocol (HTTP)]] resource API (RESTful API)
- they are not running on the same machine

### Architectural Pattern
![[Pasted image 20231104013217.png]]
- [[Single Responsibility Principle (SRP)]]

### Advantages over [[Monolithic]]
- Support for scaling & development
	- [[Microservices]] are independently deployable & scalable
>	#Example 
>	you want to implement a certain new feature at a different section of the application
>	
>	you don't need to shut down the entire server to do so
- Support for change
	- Support hot deployment of updates
- Support for reuse
	- Use same web service in multiple apps
- Support separate team development
	- Pick boundaries that match team responsibilities
- Design/Support for failure