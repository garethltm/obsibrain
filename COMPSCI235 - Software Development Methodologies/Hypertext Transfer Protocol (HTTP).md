[[Hypertext Transfer Protocol (HTTP)]] is a text-based protocol with character content of [[Hypertext Transfer Protocol (HTTP)]] messages being encoded using the [[open protocol]] & [[standard protocol]] UTF-8 encoding format

### Message types
1. Request![[Pasted image 20231101224705.png]]
2. Response![[Pasted image 20231101224730.png]]

### Method types
- [[Hypertext Transfer Protocol (HTTP)]] defines a set of methods, one of which is specified in a request message:
	- `GET` (Retrieve information)
		- REQUESTS a specified resource
	- `HEAD` (Not returning actual resource but all meta data related to the resource)
		- similar to GET, only returns meta data for the resource
		> #Example 
		> 		modification time, size, type
	- `POST` (Putting data to the server/Grant access to users) $\rightarrow$ register someone
		- REQUESTS that the named resource processes data
		- typically used to process form data
	- `PUT` (Not creating new resource; changing/updating details of an information)
		- REQUESTS that the named resource is replaced with data contained in the message body
	- DELETE
		- Re