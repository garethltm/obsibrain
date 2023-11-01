makes a better user experience

- [[Hypertext Transfer Protocol (HTTP)]] is a [[stateless]] protocol - that's why there's is a need for cookies
	- the server would know where these requests are coming from & whether they are linked
- A [[cookie]] is a unique identifier, created on the server side & sent to the browser
	- server would create a unique identifier & would send back to the browser
- It stores a key/value pair (plus optional parameters)
>	#Example 
>	username = 'Winston'

- Has several applications
>	#Example 
>	user tracking, personalization & most importantly, [[Authentication]]

- A web server can "set" a [[cookie]] into the client using the "`Set-Cookie`" response header (sending stuff in the header) & the browser then sends this [[cookie]] to the server with each subsequent [[Hypertext Transfer Protocol (HTTP)]] request using the "[[Cookie]]" request header
