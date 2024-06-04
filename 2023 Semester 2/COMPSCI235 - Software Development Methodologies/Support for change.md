Ease of change

- Large organizations, constantly have new features being finished & rolled out to production
- [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/Microservices]] - easy to iterate & implement structural changes by working in organized [[SPRINT (iteration)]]
	- putting together certain functions that have a singular purpose in a microservice
>	#Example 
>	User wants to buy stuff
>	- so you put the user & the catalogue together
- [[Monolithic]] - change cycles are tied together
	- a change made to a small part to the application, requires the entire monolith to be rebuilt & redeployed
		- might require whole website to shutdown
		- updates for 1 module would mean the entire website would be down