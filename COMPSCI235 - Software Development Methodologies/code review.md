Software professional rank [[code review]] as the number one factor for improving [[code quality]]
- if done early is better as it would be a higher price later (like interest)

A [[code review]] is a constructive review of a fellow developer's code

A required sign-off from another team member before a developer is permitted to check-in changes or new code

[[code review]] helps to reduce code defects & improve [[code quality]]

### Mechanics
- who:
	- Original developer & reviewer
		- sometimes together in person, sometimes offline
- what:
	- Reviewer gives suggestions for improvement on a logical and/or structural level, to conform to previously agreed up set of quality standards.
		- feedback leads to [[Refactoring]], followed by a 2nd [[code review]] (taking in feedback)
		- Eventually reviewer approves code
- when:
	- when code author has finished a coherent system change that is otherwise ready for check-in
		- change shouldn't be too large/too small
		- before committing the code to the repository or incorporating it into the new build

>	#Example 
>	Pull request on [[GitHub]] $\rightarrow$ prevents code from being pushed to main without [[code review]] first

### How are [[code review]] performed?
1. Meeting-based:
	- coders complete their work & meeting is called for [[code review]]
	- 