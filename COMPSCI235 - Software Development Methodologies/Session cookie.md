temporary [[cookie]]; only there while the [[session]] exists
- a time where the user is interacting with the server
	- when user logs in/out; open/close browser

1. User submits login credentials
>	#Example 
>	username & password

2. Server:
	- verifies the credentials from the [[COMPSCI235 - Software Development Methodologies/database|database]]
	- creates a temporary user [[session]]
	- issues the [[cookie]] with a sessionID

3. User sends the [[cookie]] with each subsequent request
4. Server validates the sessionID against the [[session]] store & grant access to the user
5. When user logs out, server destroys the [[session]] & clears the [[cookie]] on client site