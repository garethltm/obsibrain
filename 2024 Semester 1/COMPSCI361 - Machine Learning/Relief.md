- Instance-based heuristic for [[Attribute (Feature) selection]] 
- Intuitive algorithm

![[Pasted image 20240426173604.png]]
Uses random subset of the data instances to iteratively calculate weight values for each attribute, based on how important the attribute seems to be in discriminating between nearest neighbours in different classes.
- Larger the weight = more important is the attribute
## The basic algorithm
![[Pasted image 20240426173640.png]]
- The algorithm above is the basic version of Relief (Kira & Rendell 1992), proposed with Euclidean distance for both neighbour selections & weight updates, and weight threshold for [[Attribute (Feature) selection]] (instead of the $k$ parameter)
- If categorical attributes are in the dataset, use Hamming distance for those attributes: 
  ($dist(x,y)= 0 \ if\ x == y\ else\ 1$)
- You can replace Euclidean distance with Manhattan distance:
  ($dist(x,y)=|x)
## Summary
- Relief takes into account all attribute
	- Therefore, it cannot deal with redundancy
- Outputs weight vector that represents the importance of each attribute
