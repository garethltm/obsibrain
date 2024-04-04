- the best line (w) that minimises the distances between the point

## Objective
Linear model:
$$\huge \hat {y}\tiny {i} = \huge {wx}\tiny {i}$$
Predictions:
$$\huge \hat {y}\tiny {i} = \huge {w} \tilde{x} \tiny {i}$$
### One thing we CANNOT do:
- We can't use the same error as before:
	- It is unlikely to find a line where $\huge \hat {y}\tiny {i} = \huge {y}\tiny {i}$ for exactly many points
		- Due to noise, relationship not being quite linear or just floating-point issues
	- Best model may have $|\huge \hat {y}\tiny {i} - \huge {y}\tiny {i}\normalsize|$ is small but not exactly 0
- Instead of exactly $\huge {y}\tiny {i}$, we evaluate size of the error in prediction
- Classic way is setting slope w to minimize sum of squared errors![[Screenshot 2024-04-04 at 4.11.17 PM.png]]
- It is done because it is easy to minimize
	- we want to minimise this error because we want to find the line that approximates the best
![[Pasted image 20240404161337.png]]