- Start with $E_{test} = E_{test}$ , then add & subtract $E_{train}$ on the right:
	- ![[Pasted image 20240312221008.png]]
### How does this help?
- If $E_{approx} = E_{test}-E_{train}$ is small, then $E_{train}$ is a good approximation to $E_{test}$

### What does $E_{approx}$ ("amount of [[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]]") depend on?
- It tends to get smaller as 'n' gets larger
	- number of examples $\rightarrow$ more depth
- It tends to grow as model get more "complicated"

### This leads to a [[Fundamental Trade-Off]]:
1. $E_{train}$ : how small you can make the [[Training error]] 
2. $E_{approx}$ : how well [[Training error]] approximates the test error
#### Simple models (like [[Decision Stumps]]):
1. $E_{approx}