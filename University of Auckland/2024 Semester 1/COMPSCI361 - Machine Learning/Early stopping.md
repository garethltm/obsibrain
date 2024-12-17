Simple and popular [[Regularisation]] technic
![[Pasted image 20240607004333.png]]
Learn enough, but not too much
- avoid to end up in the high [[variance]] zone

Avoid too much training = lowest [[Validation Error]]
## When to stop
1. Monitor the performance on the validation set
	- Loss on the dev dataset (if it's at the lowest point, we STOP)
	- Additional metrics ([[Precision (Exactness)]], [[Recall (Completeness)]], etc.)
2. Trigger the early stopping
	- Simplest trigger: increase of the [[Loss Function]] compared to the last iterations
	- More elaborated ones: no change over several epochs, absolute change in a metric, average change in a metric over several epochs, reaching a specific level of performance, etc.
3. Choose the model to keep
	- Usually, keep the model from the epoch before the increase in [[Loss Function]]
