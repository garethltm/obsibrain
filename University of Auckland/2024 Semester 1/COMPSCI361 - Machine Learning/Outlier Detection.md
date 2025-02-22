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
	- **Advantages**: Effective in high-dimensional spaces, robust to [[Outlier]], can model complex relationships
	- **Disadvantages**: Requires labeled data, computationally intensive for large datasets
	- #compsci361example [[One-Class SVM (OC-SVM)]]
6. [[Clustering]] ([[k-Means]], [[DBSCAN]])
	- used to identify [[Outlier]] as points that do not fit well into any [[cluster(s)]] or form their own small [[cluster(s)]]
	- **Advantages**: Does not require labeled data, can detect groups of [[Outlier]]
	- **Disadvantages**: Choice of [[Clustering]] [[parameters]] can significantly affect results, may struggle with high-dimensional data
	- #compsci361example [[DBSCAN]] identifies [[Outlier]] as points that are in low-density regions
7. [[Principal Components Analysis (PCA)]]
	- reduces the dimensionality of data while preserving [[variance]]. [[Outlier]] can be identified by looking at the principal components and detecting points that have unusual values.
	- **Advantages**: Reduces dimensionality, highlights [[variance]] in data
	- **Disadvantages**: Sensitive to scaling, linear method may not capture complex patterns
	- #compsci361example Points that have high value in the directions of principal components can be considered [[Outlier]]
8. [[Scatter Plot]]
## Where to use [[Outlier Detection]]?
1. Anomaly Detection in Network Traffic
	- Using [[k-nearest neighbor (kNN)]] or [[Clustering]] to detect unusual patterns that may indicate security breaches
2. Fraud Detection in Financial Transactions
	- Applying [[Support Vector Machines (SVM)]] to identify fraudulent transactions that deviate from normal behavior
3. Quality Control in Manufacturing
	- Using [[Principal Components Analysis (PCA)]] to detect defective products by identifying measurements that fall outside normal ranges
4. Medical Diagnosis
	- [[Clustering]] can help identify rare diseases by finding patients whose medical records differ significantly from the norm

**Detection outliers requires domain expertise**
- You have to examine your data to see whether this data point is an [[Outlier]] or not