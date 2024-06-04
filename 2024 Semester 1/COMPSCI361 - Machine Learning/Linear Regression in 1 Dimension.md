- based on 1-feature

1. Assume we only have 1 feature (d = 1)
		#compsci361example $\huge {x}\tiny {i}$ is number of cigarettes & $\huge {y}\tiny {i}$ is number of lung cancer deaths
2. [[Linear Regression]] makes predictions $\huge \hat {y}\tiny {i}$ using a linear function of $\huge {x}\tiny {i}$ 
		$\huge \hat {y}\tiny {i}\normalsize = \huge {wx}\tiny {i}$
3. The parameter w is the weight or [[Regression]] coefficient of $\huge {x}\tiny {i}$ (similar to: y = mx + c)
		We are temporarily ignoring the y-intercept
4. As $\huge {x}\tiny {i}$ changes, slope w affects the rate that $\huge \hat {y}\tiny {i}$ increases/decreases
		![[Pasted image 20240404155947.png]]
	- Positive w: $\huge \hat {y}\tiny {i}$ increase as $\huge {x}\tiny {i}$ increases
	- Negative w: $\huge \hat {y}\tiny {i}$ decrease as $\huge {x}\tiny {i}$ increases
![[Pasted image 20240404160005.png]]
