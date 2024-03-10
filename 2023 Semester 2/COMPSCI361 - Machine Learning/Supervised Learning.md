![[Pasted image 20240229223953.png]]
Input: set of features
Output: class label

#compsci361example 
Input: a day of the week with the quantities of food
Output: whether we got sick or not

## Goal
- Use data to find a model that outputs the label based on the features
- Model predicts whether which food make you sick (even with new combination)

1. General [[Supervised Learning]] problem
	- take features of examples and corresponding labels as input
	- find a model that can accurately predict the labels of new examples
2. This is the most successful/widely used [[Machine Learning (ML)]] technique
	- #compsci361example 
	- spam filtering, optical character recognition, speech recognition, classifying tumors, etc.
3. [[Classification]]

## as Writing a program
- There are many possible [[2023 Semester 2/COMPSCI361 - Machine Learning/Decision Trees|Decision Trees]] 
	- We're going to search for one that is good at our [[Supervised Learning]] problem
- So our input = data, output = program
	- this is called "training" the [[Supervised Learning]] model
- [[Supervised Learning]] is useful when you have lots of labeled data BUT:
	1. Problem is too complicated to write a program ourselves
	2. Human expert can't explain why you assign certain labels, OR 
	3. We DON'T have a human expert for the problem