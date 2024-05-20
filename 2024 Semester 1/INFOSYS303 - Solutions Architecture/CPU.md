- We want to determine the number of virtual machines per server
- Depends on the cores available & how many vCPUs are needed per VM

$$Virtual\ Machines\ per\ Server=\frac{Cores\ Available\ on\ Server}{vCPUs\ Needed\ per\ Virtual\ Machine}$$
#infosys303example if it is determined that 2 vCPUs are needed per VM, then a server with 16 cores can provide $\frac {16}{2}=8\ VMs$

An important (design) relation to establish is how much can the capacity of a core can be split
- the answer lies on oversubscribe [[CPU]] resources in order to achieve an optimal density of virtual machines:
	- recommended sizing can be as many as 10 vCPUs per physical [[CPU core]](pCPU), depending on the workload
	- a good, conservative starting point in the design is 6vCPUs per pCPU when calculating density
- Such oversubscription is given by the ratio of virtual CPUs to physical CPUs,