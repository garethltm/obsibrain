Multiple computations happening at the same time, rather than sequentially![[Pasted image 20231101181322.png]]

Servers typically provide internal concurrency using [[thread]] & [[thread pools]]

When a request arrives, an available [[thread]] is checked out of the [[thre]] & used to handle the request; afterwards the [[thread]] is returned to the [[thread pools]]