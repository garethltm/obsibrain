A [[transaction(s)]] is the execution of a sequence of 1 or more operations on a [[COMPSCI235 - Software Development Methodologies/database|database]] to perform some higher-level function
- Partial [[transaction(s)]] are not allowed

Bundle multiple [[COMPSCI235 - Software Development Methodologies/database|database]] changes into atomic operations
- Rollback or Undo the changes if needed
	- as they are atomic in nature

>	#Example 
>	2 customers want to book a seat in a flight using a flight reservation system
>	They both try to book the same seat at the same time
>	- Problem: Concurrent multi-user access![[Pasted image 20231102105423.png]]

>	#Example 
>	You want to transfer $10,000 from your cheque account to your savings account but there is hardware or software "crash" while the operation is executing
>	- Problem: Atomicity of updates
>		- they are atomic in nature; which basically means that it cannot be broken down
>	- DBMS guarantees stability as they are using the concept of transactions![[Pasted image 20231102105731.png]]