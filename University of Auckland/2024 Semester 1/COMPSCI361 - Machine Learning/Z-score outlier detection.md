![[Pasted image 20240607013535.png]]
- The Z-score method for [[Outlier Detection]] uses a dataset's standard deviation and its mean to identify data points that are significantly different from the majority of the other data points

The Z-score for a value of $x$ in the dataset with a normal distribution with mean $\mu$ and standard deviation $\sigma$ is given by:
$$z=\frac{(x-\mu )}{\sigma}$$
- The Z-score is equal to zero when $x=\mu$
- The Z-score is $± 1$, $± 2$, or $± 3$, depending on whether $x$ is $± 1$, $± 2$, or $± 3$, respectively

A data point with a Z-score (the number of standard deviations the data point is away from the mean) of more than 3 or less than -3 is typically considered to be an [[Outlier]]. This method assumes that the data follows a normal distribution. It is a simple and widely used method for [[Outlier Detection]]m but it may not always be appropriate for data that is not normally distributed