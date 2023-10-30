- [[Greedy Descent]] with M random restarts: Each search process runs independently of the others
	- just one agent mainly
- [[Local beam Search]]: useful information is passed among the parallel search threads
	- combining the information you have
	- [[Multi-agent]] [[Environment]] so it is somewhat more faster/better in te

### Advantage
- you can have early termination on useless paths, which you can direct your attention on better potential [[solution(s)]]
#### Disadvantage
- The M searches may concentrate on one search branch after a few steps
	- You basically lose diversity because it is called [[Population-based Search]] - which defeats its main purpose