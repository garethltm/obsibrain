- Both decompositions serve the same purpose
	- Trying to evaluate how different factors affect test error
- They both lead to the same 3 conclusions
	1. Simple models can have high $E_{train}$ / bias, low $E_{approx}$ / variance
	2. Complex models can have low $E_{train}$ / bias, high $E_{approx}$ / variance
	3. As you increase n, $E_{approx}$ / variance goes down (for fixed complexity)