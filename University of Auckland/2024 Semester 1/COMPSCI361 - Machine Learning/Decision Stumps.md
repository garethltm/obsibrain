# Learning a Decision Stump: 
## 1. Search and Score
- We'll start with "[[Decision Stumps]]"
	- Simple [[Decision Tree(s)|Decision Tree(s)]] with one splitting rule based on thresholding one feature![[Pasted image 20240307151634.png]]
## How do we find the best "rule" (feature, threshold & leaf labels)?
1. Define a 'score' for the rule
2. Search for the rule with the best score
## What would you suggest as a score?
- the one that has the most correct [[classification]]
	- the cleanest ones $\rightarrow$ less errors (data is never perfect)
## 2. [[Accuracy]] Score
- Maybe most intuitive score: [[classification accuracy]]
- #compsci361example ![[Pasted image 20240307152928.png]]
- Computing [[classification accuracy]] for (egg > 1):
	- Find most common labels if we use this rule:
		1. When (egg $\gt$ 1), we were "sick" $\frac{2}{2}$
		2. When (egg $\leq$ 1), we were "not sick" $\frac{3}{4}$
	- Compute accuracy:
		- The accuracy ("score") of the rule (egg > 1) is $\frac{5}{6}$
- The "score" evaluates quality of a rule
	- We "learn" a [[Decision Stumps]] by finding the rule with the best score.
## 3. By Hand
- Let's search for the [[Decision Stumps]] maximizing [[classification]] score:
	1. First we check "baseline rule" of (we want to beat this baseline rule)
		- predicting mode (no split)
			- $\frac{3}{6}$ accuracy
	1. If (milk > 0): 
		- predict "sick" ($\frac{2}{3}$) 
		- predict "not sick" ($\frac{2}{3}$)
			- $\frac{4}{6}$ accuracy
	2. If (fish > 0):
		- predict "not sick" ($\frac{2}{3}$)
		- predict "sick" ($\frac{2}{3}$)
			- $\frac{4}{6}$ accuracy
	3. If (fish > 1.2):
		- predict "sick" ($\frac{1}{1}$)
		- predict "not sick" ($\frac{3}{5}$)
			- $\frac{5}{6}$ accuracy
	4. If (egg > 0):
		- predict "sick" ($\frac{3}{3}$)
		- predict "not sick" ($\frac{3}{3}$)
			- $\frac{6}{6}$ accuracy
	5. If (egg > 1):
		- predict "sick" ($\frac{2}{2}$)
		- predict "not sick" ($\frac{3}{4}$)
			- $\frac{5}{6}$ accuracy
- Highest-scoring rule:
	- (egg > 0) $\rightarrow$ $\frac{6}{6}$
- Notice we only need to test feature thresholds that happen in the data (we don't need other types of split because it is NOT in the dataset)
	1. There is no point in testing the rule (egg > 3)
		- it gets the "baseline" score
	2. There is no point in testing the rule (egg > 0.5)
		- it gets the (egg > 0) score
	3. Also note that we don't need to test "$\lt$", since it would give equivalent rules
## Summary
- simple [[Decision Tree(s)|Decision Tree(s)]] that is very fast to fit