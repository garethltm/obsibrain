- uses the same procedures as [[Hill-Climbing]] with following differences:
	1. When no [[uphill successors]] are present, move "[[sideways]]" 
	2. Introduce a parameter m such that only ≤ m steps we can perform  [[sideways]] moves consecutively
		- this solves the shoulder problem
- loop on at maxima
	- limit number of consecutive [[sideways]] steps
		![[Pasted image 20231022161956.png]]
		- where we can overcome the shoulder & go up towards global maximum
