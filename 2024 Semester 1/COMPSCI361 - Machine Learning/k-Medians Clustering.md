With other distances [[k-Means]] may not converge
- But we can make it converge by changing the updates so that they are minimizing an alternative objective function
	- by changing the updates = you are changing the objective function, which allows us to represent that representative example differently not with average
	- this will converge & will be the [[Optimal]] solution starting from the right initial centres
#compsci361example we can use the L1-norm as an objective:
$$
\sum_{i=1}^{n} \| w_{\hat{y}_i} - x_i \|_1 = \sum_{i=1}^{n} \sum_{j=1}^{d} | w_{\hat{y}_i}[j] - x_i[j] | 
$$
- $w_{\hat{y}_i}[j] - x_i[j]$ represents the sum of the absolute differences in each dimension ([[Manhattan distance]])
Minimizing the L1-norm objective gives the [[k-Medians Clustering]] algorithm
- Assign points to [[cluster(s)]] by finding centres with smallest L1-norm distance
- Update cluster centers as median value (dimension-wise) of each [[cluster(s)]]
	- this minimizes the L1-norm distance to all the instances in the [[cluster(s)]]

**Advantage: This approach is more robust to outliers**
