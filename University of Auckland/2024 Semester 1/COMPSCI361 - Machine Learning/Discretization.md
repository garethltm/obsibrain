- concept hierarchy climbing
## 3 types of attributes
1. Nominal - values from an unordered set #compsci361example color
	- Distances in Euclidean scale doesn't apply here
2. Ordinal - values from an ordered set #compsci361example rank
	- can be converted to Nominal/Numeric
3. Numeric - real numbers #compsci361example integers/reals
- Both Ordinal & Numeric can apply scale

[[Discretization]] divides a range of continuous attributes into intervals
1. Interval labels can then be used to replace actual data values
2. [[Discretization]] can be performed recursively on an attribute
3. Reduce data size by [[Discretization]]
4. Prepare for further analysis #compsci361example ([[classification]])
5. The resulting mined patterns are typically easier to understand
6. Mining on different level of data abstraction (concept hierarchies)
- Continuous values to Binary values with [[Decision Tree(s)]] (0 or 1)

## Methods
1. Top-down (splitting) vs. Bottom-up (merging) - which direction it proceeds
2. [[Supervised Learning]] vs. [[Unsupervised Learning]] (Are you taking into account the target variable) - class information usage
#compsci361example 
1. [[Binning]] - top-down split, [[Unsupervised Learning]]
2. Histogram analysis - top-down split, [[Unsupervised Learning]]
3. [[Clustering]] analysis - top-down split /bottom-up merge, [[Unsupervised Learning]]
4. [[Decision Tree(s)]] analysis - top-down split, [[Supervised Learning]]
5. [[Correlation analysis]] - bottom-up merge, [[Supervised Learning]]