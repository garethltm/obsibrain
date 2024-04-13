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