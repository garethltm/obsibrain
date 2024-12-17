![[Pasted image 20231102103106.png]]
>	#Example 
	1. Users - CRUD operations
		- Can the repository:
			- Add a user
			- Retrieve a user by username
			- Return null when asked to retrieve a non-existent user
	2. Tags
		- Can the repository:
			- Add a tag
			- Retrieve all tags
	3. Comments
		- Can the repository:
			- Add a comment
			- Reject a comment that's not correctly associated with a `User` & an `Article`
			- Retrieve all comments
	4. Articles
		- Can the repository:
			- Add an article
			- Return the number of articles stored
			- Retrieve an article by id
			- Retrieve a list of articles corresponding a list of article ids
			- Retrieve the first & last articles stored
			- Return an empty list when asked for articles on a date for which there are no articles
			- Retrieve a list of article ids for articles tagged with a particular tag
			- Given an article, return the closes preceding date that has articles
			- Given an article, return close successive date that has articles![[Pasted image 20231102103629.png]]

Related to: [[Unit Testing]]