## Main Idea
- never expand a [[state(s)]] twice (if not necessary)

### How to implement:
- [[Search Tree]] + set of expanded states (”closed set”) not the same as [[closed list]]?
- Expand the [[search tree]] node-by-node, but…
- Before expanding a node, check to make sure its state has never been expanded before
    - If not new, skip it,
    - If new, expand and add to closed set

Important: store the closed set as a set (hash table), not a list