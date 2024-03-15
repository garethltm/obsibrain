1. measure of variance
	- how sensitive we are to training data
2. measure of bias
	- how low can we make the [[Training error]]
3. measure of noise
	- how low can any model make [[test error]]

- Assume $\tilde{y} \tiny{i} \normalsize = \tilde{y} \tiny{i} \normalsize + \in$ , where $\in$ has mean 0 & variance $\sigma ^2$
- Assumes we have a learner that can take n training examples & use these to make predictions $\hat{y} \tiny{i}$

### Expected squared [[test error]] in this setting is![[Pasted image 20240312223800.png]]
- Where expectations are taken over possible training sets of n examples
- Bias is expected error due to having wrong model
- Variance is expected error due to sensitivity to the training set
- Noise ([[irreducible error]]) is the best we can hope for given the noise ($E_{best}$)