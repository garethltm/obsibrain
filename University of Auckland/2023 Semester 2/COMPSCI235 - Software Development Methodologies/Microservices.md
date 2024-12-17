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
- [[Support for scaling & development]]
	- [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/Microservices]] are independently deployable & scalable
>	#Example 
>	you want to implement a certain new feature at a different section of the application
>	
>	you don't need to shut down the entire server to do so
- [[Support for change]]
	- Support hot deployment of updates
- [[Support for reuse]]
	- Use same web service in multiple apps
- [[Support separate team development]]
	- Pick boundaries that match team responsibilities
- [[Design or Support for failure]]
	- one complexity to handle with [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/Microservices]]

### Challenges
- Increased complexity
	- not always the best solution for an application
		- if simple/small user base $\rightarrow$ [[Monolithic]] might be better
	- hard to divide them to smaller [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/Microservices]]
- Data consistency
	- due to each service having its own [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/database|database]]
		- potential redundancy - duplicates
- Greater security risks
	- more APIs which can lead to more open ports
- Different programming languages
	- different languages make deployment/maintenance more difficult
		- different [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/Microservices]] generally have different languages used to communicate with each other
- Performance (one of the major drawbacks)
	- remote procedure call
		- it basically takes time to get/fetch data it needs from other [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/Microservices]] to achieve its goal

# Conclusion
![[Pasted image 20231104020521.png]]
[[Monolithic]] architecture is a traditional solution for building applications

There are various reasons for using [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/Microservices]] architecture - but there are limitations & downsides to consider as well

[[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/Microservices]] architecture requires:
- careful planning
- enormous effort
- team resources
- skills


