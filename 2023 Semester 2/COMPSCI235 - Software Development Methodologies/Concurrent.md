Multiple computations happening at the same time, rather than sequentially
- which solves the multiple user problem
	![[Pasted image 20231101181322.png]]

Servers typically provide internal concurrency using [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/thread]] & [[thread pools]]

When a request arrives, an available [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/thread]] is checked out of the [[thread pools]] & used to handle the request; afterwards the [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/thread]] is returned to the [[thread pools]]
	![[Pasted image 20231101181741.png]]

[[2023 Semester 2/COMPSCI235 - Software Development Methodologies/thread]] compete for use of the machine's processor(s)
	![[Pasted image 20231101181810.png]]

There might be inconsistency problems with multithread
- [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/thread]] may clash getting shared resources