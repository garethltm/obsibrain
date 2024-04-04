- the best line (w) that minimises the distances between the point

Linear model:
$$\huge \hat {y}\tiny {i} = \huge {wx}\tiny {i}$$
Predictions:
$$\huge \hat {y}\tiny {i} = \huge {w} \tilde{x} \tiny {i}$$
### One thing we CANNOT do:
- We can't use the same error as before:
	- It is unlikely to find a line where $\huge \hat {y}\tiny {i} = \huge {y}\tiny {i}$ for exactly many points
		- Due to noise, relationship not being quite linear or just floating-point issues
	- Best model may have $|\huge \hat {y}\tiny {i} - \huge {y}\tiny {i}$