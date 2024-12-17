- combines [[Randomly under-sampling the majority class]] & [[Randomly over-sampling the minority class]]
- creates new examples that don't exist in your data - expands the minority class
	- generally, creates new artificial instances
### Process
- Find pairs of instances, in the minority class that are closest to each other
	- nearest neighbours within the class
- Create a new instance between these instances, assign it to the minority class

![[Pasted image 20240424170705.png]]
## Assumption
1. it is a clean cluster $\rightarrow$ there is a clean separation between the 2 classes
2. if mixed $\rightarrow$ it is less likely that the green points would belong to the red classes