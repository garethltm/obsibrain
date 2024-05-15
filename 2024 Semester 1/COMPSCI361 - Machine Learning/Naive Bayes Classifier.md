- assumes all attributes describing $X$ are [[conditionally independent]] given $Y$
	- dramatically reduces the number of [[parameters]] that must be estimated to learn the [[classifier(s)]] (meaning smaller [[training data]] sets are sufficient for the learning task)

Applies to learning tasks where each instance x is described by a conjunction of attribute values $<a\tiny{1} \normalsize , a\tiny{2} \normalsize, \dots ,a\tiny{n}>$ & where the target function $f(x)$ can take on any value from some finite set V
- [[Naive Bayes Classifier]] solves the spam problem
- $<a\tiny{1} \normalsize , a\tiny{2} \normalsize, \dots ,a\tiny{n}>$ is the [[posterior evidence (posterior probability)]] given the attribute values you have seen for that particular instance
	- #compsci361example can represent color, height,...

- the most probable target value is:
$$
V_{\text{MAP}} = \underset{v_j \in V}{\operatorname{arg\,max}} \ P(v_j | a_1, a_2, ..., a_n)
$$

$$= \underset{v_j \in V}{\operatorname{arg\,max}} \ \frac{P(a_1, a_2, ..., a_n | v_j)P(v_j)}{P(a_1, a_2, ..., a_n)}\\
$$
$$= \underset{v_j \in V}{\operatorname{arg\,max}} \ P(a_1, a_2, ..., a_n | v_j)P(v_j)$$
- $P(a_1, a_2, ..., a_n | v_j)P(v_j)$ = joint distribution & class values $\times$ posterior probability of that class
- We can remove $P(a_1, a_2, ..., a_n)$ as normalisation is not necessary
#compsci361example Given [[training data]] D, $P(v_j)$ can be estimated by counting the frequency of $v_j$ in D:
- However, it is not feasible to estimate $P(a_1, a_2, ..., a_n | v_j)$ as you would need to calculate as many terms as there is needed as how many possible values, then all would mean **all possible instances**
	- Number of these terms is |all possible instances| $\times$ |V| (which could be exponential)
## Simplification
- Assumption: Attribute values are [[conditionally independent]] given the target value
- Absolute independence of X & Y
	- $P(X,Y)=P(X|Y)P(Y)=P(X)P(Y)$
	- given you have seen $Y$, does it give any extra information on $X$ $\rightarrow$ NO
- Conditional independence of X & Y given Z
	- $P(X,Y|Z)=P(X|Y,Z)P(Y|Z)=P(X|Z)P(Y|Z)$
- Hence, $P(a_1, a_2, ..., a_n|v_j) = \prod_{i} P(a_i|y_j)$
	- you can just write it as a product of n different simple conditional probabilities
-  Hence, number of terms is |distinct attribute values| $\times$ |V| + |V|
- No explicit search through [[Hypothesis Space]] H, just counting frequencies, where V = number of classes in the dataset
- If the above assumption is correct, [[Naive Bayes]] classifications are [[Maximum A Posteriori (MAP) Hypothesis]] [[classification]]
$$
v_{\text{NB}} = \underset{v_j \in V}{\operatorname{arg\,max}} \ P(v_j) \prod_{i} P(a_i | v_j)
$$


#compsci361example We want to learn to discriminate object labeled + from objects labeled - using measurements for 3 categorical features. You are given the following objects

![[Pasted image 20240502160735.png]]
## Test1![[Pasted image 20240502161551.png]]
- Assume the features describing the object are independent of tis class
- Calculate 2 [[posterior evidence (posterior probability)]] for each test example, before we can make. decision ![[Pasted image 20240502161004.png]]
- which outputs:![[Pasted image 20240502161144.png]]
## Test2![[Pasted image 20240502161610.png]]
- Training phase outputs following [[2024 Semester 1/COMPSCI361 - Machine Learning/Probability|Probability]] estimates (tables below) used in testing phase to classify new examples![[Pasted image 20240502161432.png]]
- Issue: Observed fractions are poor estimates when we have small training set & large number of attribute values. When these are zero they will dominate the calculations for all test example described with that specific attribute value

#compsci361questions 
## How to solve this issue
- Training phase using [[Estimating Probabilities - Laplace Smoothing]] outputs following [[2024 Semester 1/COMPSCI361 - Machine Learning/Probability|Probability]] estimates![[Pasted image 20240502161845.png]]
- Conditional probability estimates (no smoothing) $P(A_i = a_i | v_j) = \frac{n_{ij}}{n_j}$ where 
	- $n_j$ is the number of training examples with class label $v_j$
	- $n_{ij}$ is the number of training examples with class label $v_j$ & attribute value $a_i$
- [[Estimating Probabilities - Laplace Smoothing]] $P(A_i = a_i | v_j)=\frac {n_{ij} +1}{n_{j} +m}$ where 
	- $m$ is the number of unique values attribute $A_i$ can have
- **Test2** [[classification]] is based on [[Estimating Probabilities - Laplace Smoothing]] estimates
## Test3
![[Pasted image 20240502162534.png]]
- Training phase using [[Estimating Probabilities - Laplace Smoothing]] outputs the following [[2024 Semester 1/COMPSCI361 - Machine Learning/Probability|Probability]] estimates![[Pasted image 20240502162459.png]]
- Missing values doesn't affect [[Bayesian Learning]]
- Missing attribute values in test examples: just omit those attribute values in the calculations
- **Test3** [[classification]] based on [[Estimating Probabilities - Laplace Smoothing]] estimates![[Pasted image 20240502162930.png]]
## Discussion
#compsci361questions 
Are [[Naive Bayes Classifier]] affected/robust to:
- isolated noise example?
	- class labels are different, features same (you should not rely on a single instance $\rightarrow$ [[Bayesian Learning]] fixes)
- irrelevant attributes?
	- doesn't influence as much because the contribution would be similar for both classes (If it is not really related to your class (random), most likely not do anything) - randomness would cancel out
- missing values?
	- doesn't affect - [[Estimating Probabilities - Laplace Smoothing]]
- correlated attributes?
	- can be an issue if they are supposed to be a combined instance
	- #compsci361example 'Machine' 'Learning' $\ne$ 'Machine Learning'
## Summary
- [[Naive Bayes]]
## Application
