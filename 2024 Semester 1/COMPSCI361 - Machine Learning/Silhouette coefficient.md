- balance between 2 things
- A measure for distance within a [[cluster(s)]] and between [[cluster(s)]]
- Range [-1,1]. More positive, better [[cluster(s)]]$$
s(x) = \frac{b(x) - a(x)}{\max(a(x), b(x))}
$$
	- $a(x)$ is the mean distance between a point $x$ and all other points in the same [[cluster(s)]] 
		- (how compact is the [[cluster(s)]] $C_i$ to which $x$ belongs)
	- $b(x)$ is the mean distance between a point $x$ & all other points in the nearest [[cluster(s)]] 
		- (how separated is the [[cluster(s)]] $C_i$ to which $x$ belongs)
	- Fitness of [[cluster(s)]] $C_i$ in given [[Clustering]] can be measured by the average [[Silhouette coefficient]] value of all points in the [[cluster(s)]]
## Visualized [[Silhouette coefficient]]
- Typically we sort & plot $s(x)$ for each instance, grouped by [[cluster(s)]]![[Pasted image 20240604173656.png]]
- Almost all points have high $s(x)$, which means that they are much closer, on average, to the other members of their [[cluster(s)]] than to the members of the neighbouring [[cluster(s)]]