![[Pasted image 20240605115223.png]]
Given a new data point $\vec {x}$, we use the learned [[Support Vector Machines (SVM)]] [[classifier(s)]] ($\vec {w}$ and $b$) to derive the class label as follows:
1. Primal Form$$
f(x) = 
\begin{cases} 
+1 & \text{if } \vec{w} \cdot \vec{x} + b > 0 \\
-1 & \text{if } \vec{w} \cdot \vec{x} + b \leq 0 
\end{cases}
$$
2. Dual form$$
f(x) = 
\begin{cases} 
+1 & \text{if } \sum_{x_i \in ESV} a_i y_i (x_i \cdot x) + b > 0, \\
-1 & \text{if } \sum_{x_i \in ESV} a_i y_i (x_i \cdot x) + b < 0.
\end{cases}
$$

#compsci361example ![[Pasted image 20240605115418.png]]