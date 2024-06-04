With other distances [[k-Means Algorithm]] may not converge
- But we can make it converge by changing the updates so that they are minimizing an alternative objective function
	- this will converge & will be the [[Optimal]] solution starting from the right initial centres
#compsci361example we can use the L1-norm as an objective:
$$
\sum_{i=1}^{n} \| w_{\hat{y}_i} - x_i \|_1 = \sum_{i=1}^{n} \sum_{j=1}^{d} | w_{\hat{y}_i}[j] - x_i[j] | 
$$
