- Most common score in practise is [[Information gain]]
	- Choose split that decreases [[entropy]] of labels the most![[Pasted image 20240307170251.png]]
- [[Information gain]] for baseline rule ("do nothing") is 0
	- Infogain is large if labels are "more predictable" ("less random") in next layer
- Even if it does not increase [[classification accuracy]] at one depth, we hope that it makes the [[classification]] easier at the next depth
## Summary
- splitting score based on decreasing [[entropy]]