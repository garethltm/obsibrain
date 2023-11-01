- As an app developer, we want to only focus on the logic rather than getting stuck with hardware/low level details
	- we'd like some help in the way of abstractions for [[Hypertext Transfer Protocol (HTTP)]], network programming & multithreading

- [[Middleware]] is a layer of [[software]] that sits between application code & the operating system
	- acting like an interface
	- provides some sort of **programming abstraction** (issues & complexity are usually hidden from application developer)
	>	#Example 
	>	remote method invocation, web frameworks, etc.

	- Provides infrastructure to take care of the low-level concerns
	>	#Example 
	>	protocols, sockets or process/thread management
	
	- Masks [[Heterogeneous]]
		- as we know that there are different types of hardware we will be running our application on (using [[Middleware]] usually prevents this)

## Benefits
- Reuse
- Portability
- Interoperability - [[Middleware]] acting as an interface