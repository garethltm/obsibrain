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
		1. When (egg $\gt$ 1), we were "sick" $\frac{2}{2}$
		2. When (egg $\leq$ 1), we were "not sick" $\frac{3}{4}$
	- Compute accuracy:
		- The accuracy ("score") of the rule (egg > 1) is $\frac{5}{6}$
- The "score" evaluates quality of a rule
	- We "learn" a decision stump by finding the rule with the best score.

## 3. By Hand
- Let's search for the [[Decision Stumps]] maximizing classification score:
	1. First we check "baseline rule" of 
		- predicting mode (no split)
		- $\frac{3}{6}$ accuracy
	2. If (milk > 0): 
		- predict "sick" ($\frac{2}{3}$) 
		- predict "not sick" ($\frac{2}{3}$)
		- $\frac{4}{6}$ accuracy
	3. If (fish > 0):
		- predict "not sick" ($\frac{2}{3}$)
		- predict "sick" ($\frac{2}{3}$)
		- $\frac{4}{6}$ accuracy
	4. If (fish > 1.2):
		- predict "sick" ($\frac{1}{1}$)
		- predict "not sick"