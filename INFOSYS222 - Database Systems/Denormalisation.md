- efficiency of **`ADD`/`UPDATE`/`DELETE`** VS **`READ`**
- [[Operations]] that requires faster **`ADD`/`UPDATE`/`DELETE`**
	good for banking systems
- [[Analytics]] requires faster **`READ`**

### Compromise:
1. Derived [[Attribute(s)]] - avoid run-time computation
2. Merge 1:1 [[Relationship]] - avoid run-time joins
3. Store Values(s) for relevant [[Keys]] - avoid run-time joins