- simple models consisting of:
	- a nested sequence of "if-else" decisions based on the features (splitting rules)
	- a class label as a return value at the end of each sequence
![[Pasted image 20240301115225.png]]

## Which score function should a decision tree use?
In terms of accuracy
- You generally want a shorter one because it generalises more - to adapt to more cases
	- you would usually make splits, decisions and patterns that occur which aren't really useful for the data
- For the leafs: no issue
- For internal nodes: not the best choice
What happens if no simple rule improves accuracy?
- this doesn't necessarily mean we should stop - it might just mean that it is just a split
Most common score in practice is "information gain"
- Choose the split that decreases [[entropy]] of labels the most

Related to: [[COMPSCI367 - Artificial Intelligence/week11/Decision Trees|Decision Trees]]