- simple models consisting of:
	- a nested sequence of "if-else" decisions based on the features (splitting rules)
	- a class label as a return value at the end of each sequence
![[Pasted image 20240301115225.png]]

## Which score function should a decision tree use?
In terms of accuracy
- You generally want a shorter one because it generalises more - to adapt to more cases
	- you would usually make splits, decisions and patterns that occur which aren't really useful for the data
- For the leaves: no issue
- For internal nodes: not the best choice
What happens if no simple rule improves accuracy?
- this doesn't necessarily mean we should stop - it might just mean that it is just a split
Most common score in practice is "information gain"
- Choose the split that decreases [[entropy]] of labels the most

### Advantages of [[Decision Tree(s)|Decision Tree(s)]]
1. Easy to implement
2. Interpretable
3. Learning is fast, prediction is very fast
4. Can elegantly handle a small number missing values during training
### Disadvantages of [[Decision Tree(s)|Decision Tree(s)]]
1. Hard to find optimal set of rules
	- Will never find the model potentially
2. [[Greedy recursive splitting]] often not accurate, requires very deep trees

## Summary
- predicting a label using a sequence of simple rules

Related to: [[2023 Semester 2/COMPSCI367 - Artificial Intelligence/week11/Decision Trees|Decision Trees]]