## Why study the [[Outlier Detection]]?
- To ensure that the trained model generalizes well to valid range of test inputs, it's important to detect and remove [[Outlier]]
- In the [[Machine Learning (ML)]] pipeline, [[Data cleaning]] and [[Data Preprocessing]] is an important step as it helps you better understand the data. During this step, you deal with [[Incomplete (Missing) Data]], detect [[Outlier]] and more.
## Statistical methods for [[Outlier Detection]]
1. [[Z-score outlier detection]]
2. [[Interquartile Range Outlier Detection (IQR)]]
3. [[k-nearest neighbor (kNN)]]
	- identifies [[Outlier]] as data points whose $K$ [[nearest neighbor(s)]] are far away from there
		1. Fix a $K$-value
		2. For each data, find its $K$ - [[nearest neighbor(s)]] and calculate the cumulative distance of this data to all $K$ neighbors
		3. Ranking all data according to their cumulative distances
		4. Treat the data points as [[Outlier]] whose $K$ [[nearest neighbor(s)]] are far away from them
4. [[Local Outlier Factor (LOF)]]
5. [[Support Vector Machines (SVM)]]
	- can be adapted for [[Outlier Detection]] by identifying a [[decision boundary]] that separates normal data points from [[Outlier]]
	- Advantages: Effective in high-dimensional spaces, robust to [[Outlier]], can model complex relationships
	- Disadvantages: Requires labeled data, computationally intensive for large datasets
	- #compsci361example [[One-Class SVM]]