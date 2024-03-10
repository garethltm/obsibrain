![[Pasted image 20231103165721.png]]
[[eXtreme Programming (XP)]] is one of several popular [[AGILE]] development processes.

"XP is a lightweight methology for small to medium sized teams developing [[software]] in the face of vague or rapidly changing requirements"

## 5 Core Values
core values that you think that are most important for your team to deliver the highest quality product
1. Communication
	- Open & Transport communication
2. Simplicity
	- Build what is NEEDED
3. Feedback
	- Customer Onsite
4. Courage
	- to adapt to change
5. Respect
	- open to taking criticism & resolving conflicts in a respectful manner

## 12 Principles
![[Pasted image 20231103170120.png]]

#### Main focus
![[Pasted image 20231103170153.png]]
1. Testing (Test are written prior to code)
	- the developers continually write [[Unit Testing]] code, which need to pass for the development to continue
	- the customers write tests to verify that the features are implemented
	- tests are automated ([[Automated Testing]]) so that they become part of the system can be continuously run to ensure the working of the system
2. Pair programming (Driver & Passenger roles)
	- all production [[software]] is built by 2 programmers, sitting side by side & performing [[code quality]] checks, at the same machine
3. [[Continuous Integration (CI)]] (committing to the main line)
	- keep system fully integrated at all times by committing multiple builds each day
		- not deviating from the main line
4. [[Refactoring]] (Code is continuously refactored)
	- iterative refinement of the internal program design
5. Short Releases (Release new versions in short cycles)
	- put a simple system into production quickly & then release new versions in very short cycles
6. Coding Standards (Code is consistent)
	- follow a common coding standard, so that all the code in the system looks as if it was written by a single (competent) individual

![[Pasted image 20231103170921.png]]
1. Planning
	- Begins with the creation of a set of stories ([[user stories]])
	- each story is written by the customer & is placed on an index card
	- the customer assigns a value (priority) to the story
	- [[AGILE]] team assesses each story & assigns a cost
	- Stories are grouped for a deliverable increment
	- A commitment is made on delivery date
	- After the first increment "project velocity" is used to help define subsequent delivery dates for other increments
2. Design
	- Follows the "keep it simple" principle
	- Encourage the use of [[Class Responsibility Collaborator (CRC) cards]]
	- For difficult design problems, suggests the creation of "spike solutions" - a design prototype
	- Encourages "[[Refactoring]]"
	- Design occurs both before & after coding commences
3. Coding
	- Recommends the construction of a series of [[Unit Testing]] codes for each of the stories before coding commences
	- Encourages "[[pair programming]]"
	- Need continuous integration with other portions (stories) of the [[software]], which provides a "smoke testing" environment
4. Testing
	- [[Unit Testing]] should be implemented using a framework to make testing automated ([[Automated Testing]]). This encourages a regression testing strategy
	- [[Integration Testing]] & Validation Testing can occur on a daily basis
	- [[Acceptance Testing]]