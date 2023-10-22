- [[Hill-Climbing with side-way moves]]

1. No [[sideways]] moves:
	- Succeeds w/ probability = 0.14
	- Average number of moves per trial:
		- 4 when succeeding
		- 3 when getting stuck
	- Expected total number of moves needed:
			$\frac {3(1-p)} {p+4}$ = ~***22 moves***
2. Allow 100 [[sideways]] moves:
	- Succeeds w/ probability = 0.94
	- Average number of moves per trial:
		- 21 when succeeding, 65 when getting stuck
	- Expected total number of moves needed:
			$\frac {65(1-p)}{p+21}$
			