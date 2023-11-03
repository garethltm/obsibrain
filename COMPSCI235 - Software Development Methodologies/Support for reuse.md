Goal
- to have ZERO coupling between [[Microservices]], aside from their shared [[Interfaces]]
	- allows the [[Microservices]] to be reused independently ([[Single Responsibility Principle (SRP)]])
		- you can plug/unplug without breaking the application (replacing 1 part without affecting the others)![[Pasted image 20231104015416.png]]

- Large organizations may have many internal products that all depend on a similar [[core service]]
- Would like to be able to build functionality once, reuse in many places