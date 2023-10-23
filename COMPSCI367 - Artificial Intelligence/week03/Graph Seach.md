## Main Idea
- never expand a state twice (if not necessary)

### How to implement:
- [[tree]] + set of expanded states (”closed set”)
- Expand the search tree node-by-node, but…
- Before expanding a node, check to make sure its state has never been expanded before
    - If not new, skip it,
    - If new, expand and add to closed set

Important: store the closed set as a set (hash table), not a list

Can graph search wreck completeness? Why/why not?

How about optimality?