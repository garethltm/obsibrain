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
2. $E_{approx}$ : how well [[Training error]] approximates the [[test error]]
#### Simple models (like [[Decision Stumps]]):
1. $E_{approx}$ : is low (not very sensitive to training set)
	- too generalised, low accuracy
2. But $E_{train}$ might be high
#### Complex models (like deep [[Decision Tree(s)]])
1. $E_{train}$ : can be low
	- too specific, high accuracy
2. But $E_{approx}$ might be high (very sensitive to training set)

#### [[Training error]] vs [[test error]] for choosing depth:
1. [[Training error]] is high for low depth (underfitting)
2. [[Training error]] gets better with depth
3. [[Test error]] initially goes down, but eventually increases ([[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]])![[Pasted image 20240312222120.png]]