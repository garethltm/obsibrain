Shown using solid connector lines
- Relationships generally affect 2 tables
![[Pasted image 20231102151726.png]]
### Types of relationships
- One-to-one
	- Where both tables should be associated with each other based on only one matching row
>	#Example 
>	"One person can have one passport"
- One-to-many
	- Where a row from one table can have multiple matching rows in another table
>	#Example 
>	"A publisher can publish multiple books"![[Pasted image 20231102151932.png]]
- Many-to-many
	- Break into 2 one-to-many relationships
>	#Example 
>	"Books & authors"![[Pasted image 20231102151808.png]]![[Pasted image 20231102152008.png]]

- [[Relationships]] are implemented using Foreign Keys
- The Foreign Key is a constraint
	- makes sure that a value in one relation MUST appear in another relation