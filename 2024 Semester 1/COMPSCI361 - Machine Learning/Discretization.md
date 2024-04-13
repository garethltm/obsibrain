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
4. Prepare for further analysis #compsci361example ([[Classification]])
5. The resulting mined patterns are typically easier to understand
6. Mining on different level of data abstraction (concept hierarchies)
- Continuous values to Binary values with [[Decision Tree(s)]] (0 or 1)

## Methods
1. Top-down vs. 