![[Pasted image 20240607014820.png]]
an efficient way to perform [[Outlier Detection]] on moderately high dimensional datasets is to use the [[Local Outlier Factor (LOF)]] algorithm

[[Local Outlier Factor (LOF)]] computes a score (local outlier factor) reflecting the degree of abnormality of the observations. It measures the local density deviation of a given data point with respect to its neighbors.
## Idea
to detect the samples that have a substantially lower density than their neighbors
## In practice
the local density is obtained from the [[k-nearest neighbor (kNN)]] (cumulative distance of $K$ neighbors). The LOF score of an observation is equal to the ratio of the average local density of its $K$ [[nearest neighbor(s)]] and its local density:
- a normal instance is expected to have a local density similar to that of its neighbors
- abnormal data are expected to have much smaller local density