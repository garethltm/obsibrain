an iterative refinement of the internal program design which doesn't affect the functionality

***"A change made to the internal structure of software to make it easier to understand & cheaper to modify without changing its observable behavior"***

Making changes to the code that:
- don't change observable behavior 
	- all [[software]] still pass - logic is essentially the same
- remove duplication or needless complexity
- enhance [[software]] quality
- make the code flexible, simpler, changeable & understandable

If not [[Refactoring]], you are incurring a [[technical debt]] which would cost more later

## General Refactoring Process
![[Pasted image 20231104010830.png]]
- do [[Test-driven development (AGILE practice)]] + [[Refactoring]]

- Make sure your tests pass
- Find some code that "smells"
- Determine how to simplify this code
- Make the simplifications
- Run test to ensure things still work correctly
- Repeat the simplify/test cycle until the smell is gone

## Performing 