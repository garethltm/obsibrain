handle small measurement error

#compsci361example ![[Pasted image 20240413222810.png]]

#compsci361example 
Sorted data: $4, 8, 9, 15, 21, 21, 24, 25, 26, 28, 29, 34$
Partition into equal-frequency (equi-depth) bins:
1. $4, 8, 9, 15$
2. $21, 21, 24, 25$
3. $26, 28, 29, 34$

Smoothing by:
- bin means
	1. $9, 9, 9, 9$
	2. $23, 23, 23, 23$
	3. $29, 29, 29, 29$
- bin boundaries
	1. $4, 4, 4, 15$
	2. $21, 21, 25, 25$
	3. $26, 26, 26, 34$
## Potential Problem
- Skewed distribution grouping vastly different values together
	- #compsci361example grouping 10 year olds & 30 years together
## [[Discretization]]
1. Equal-width (distance) partitioning
	- You define each bin to cover the same length (100 samples $\rightarrow$ 10 bins each)
	- Divides the range into N intervals of equal size: uniform grid
	- If A & B are the lowest & highest values of the attribute, the width of intervals will be $W = \frac {B-A}{N}$
		- Problem: 
			- Outliers may dominate presentation
			- Skewed data is not handled well
2. Equal-depth (frequency) partitioning
	- Divides the range into N intervals, each containing approximately same number of s