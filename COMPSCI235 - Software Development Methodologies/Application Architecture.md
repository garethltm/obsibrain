![[Pasted image 20231101235727.png]]
- Each module has a well-defined responsibility ([[Single Responsibility Principle (SRP)]])
- Request handlers (`view layer`) are concerned with:
	- extracting information from [[Hypertext Transfer Protocol (HTTP)]] requests
	- creating [[Hypertext Markup Language (HTML)]]
- The `service layer` is responsible for:
	- fetching data from the repository
	- processing requests using the data
	- updating repository data
		- FORM, login...

## Full Architecture
![[Pasted image 20231102000143.png]]

### Benefits from the [[Application Architecture]]
The `view layer` has no dependency on the domain model
- certain changes to the implementation of the domain model won't necessitate change to the view layer

[[Flask Blueprint]] implementations maintain a separation of `view layer` & `service layer` concerns
- The service component of a [[Flask Blueprint]] can be reused with different views
>	#Example 
>	views that generate JSON or XML instead of HTML would reuse the service components
>	(you can basically just change the view layer & it would*)