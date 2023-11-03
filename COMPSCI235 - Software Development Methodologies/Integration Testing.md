making sure that the 2 functions are working well together (basically checking connections)

[[testing]] independent modules together

We have written unit tests for several components
- `Domain model`
- `Repository`
- `Service layer`
![[Pasted image 20231102103928.png]]

We now want to test that the components work together & that the Web application as a whole behaves as expected
- this involves writing integration tests
>	#Example 
>	password > 8 char
>	
>	A car is made up of many components
>		if the car moves, all of the necessary components work

- Individual units are combined & tested to verify if they are working as they intend to when integrated
- Main aim here is to test the [[Interfaces]] between the modules
- Test drivers & test [[stub]] are used to assist in [[Integration Testing]]
- testing 2 or more [[INFOSYS222 - Database Systems/Dependency|Dependency]] [[software]] components as a group

- a [[software]] application can be tested by similarly running it, inputting values & seeing if it behaves as expected
- [[Integration Testing]] is useful but it is only complimentary to [[Unit Testing]] - where [[Unit Testing]] tests individual components in isolation
	- we should do [[Unit Testing]] first

Any of [[Black Box Testing]], [[White Box Testing]] or [[Gray Box Testing]] methods can be used