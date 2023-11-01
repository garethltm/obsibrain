Multiple computations happening at the same time, rather than sequentially
- which solves the multiple user problem![[Pasted image 20231101181322.png]]

Servers typically provide internal concurrency using [[thread]] & [[thread pools]]

When a request arrives, an available [[thread]] is checked out of the [[thread pools]] & used to handle the request; afterwards the [[thread]] is returned to the [[thread pools]]

[[thread]] compete for use of the machine's processor(s)