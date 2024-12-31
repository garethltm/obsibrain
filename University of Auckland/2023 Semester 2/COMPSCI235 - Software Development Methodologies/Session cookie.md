temporary [[cookie]]; only there while the [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/session]] exists
- a time where the user is interacting with the server
	- when user logs in/out; open/close browser

1. User submits login credentials
>	#Example 
>	username & password

2. Server:
	- verifies the credentials from the [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/database|database]]
	- creates a temporary user [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/session]]
	- issues the [[cookie]] with a sessionID

3. User sends the [[cookie]] with each subsequent request
4. Server validates the sessionID against the [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/session]] store & grant access to the user
5. When user logs out, server destroys the [[University of Auckland/2023 Semester 2/COMPSCI235 - Software Development Methodologies/session]] & clears the [[cookie]] on client site
![[Pasted image 20231102011233.png]]