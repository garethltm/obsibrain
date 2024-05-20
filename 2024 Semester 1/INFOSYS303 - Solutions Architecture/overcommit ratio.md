- not a conservative approach
- the [[overcommit ratio]] is a design decision. This means our previous (conservative) formula can be modified by:
$$Virtual\ Machines\ per\ Server=\frac{Cores\ Available\ on\ Server}{vCPUs\ Needed\ per\ Virtual\ Machine}\times {Overcommit\ Ratio}$$
#infosys303example if the overcommit ratio is 6, the previous example would advise a number of $8\times 6$