# Learning a Decision Stump: 
## 1. Search and Score
- We'll start with "[[decision stumps]]"
	- Simple [[COMPSCI361 - Machine Learning/Decision Trees|Decision Trees]] with one splitting rule based on thresholding one feature![[Pasted image 20240307151634.png]]

## How do we find the best "rule" (feature, threshold & leaf labels)?
1. Define a 'score' for the rule
2. Search for the rule with the best score

## What would you suggest as a score?
- the one that has the most correct classification
	- the cleanest ones $\rightarrow$ less errors (data is never perfect)

## 2. Accuracy Score
- Maybe most intuitive score: [[classification accuracy]]
- #compsci361example ![[Pasted image 20240307152928.png]]
- Computing classification accuracy for (egg > 1):
	- Find most common labels if we use this rule:
		1. When (egg > 1), we were "sick" 2 times out of 2