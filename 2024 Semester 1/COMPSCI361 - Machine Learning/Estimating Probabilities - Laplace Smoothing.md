- When we don't find certain words in your dataset

$$P(x_i = w|c) = \frac{count(w, c)}{\sum_{x \in X} count(x, c)}$$
## What if $count(w, c) = 0$?
Solution: Simply add a constant
$P(x_i = w|c) = \frac{count(w, c) + 1}{\sum_{x \in F} count(x, c) + 1}$
$P(x_i = w|c) = \frac{count(w, c) + 1}{\sum_{x \in F} count(x, c) + |X|}$

