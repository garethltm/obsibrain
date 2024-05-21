- not a conservative approach
- the [[overcommit ratio]] is a design decision. This means our previous (conservative) formula can be modified by:
$$Virtual\ Machines\ per\ Server=\frac{Cores\ Available\ on\ Server}{vCPUs\ Needed\ per\ Virtual\ Machine}\times {Overcommit\ Ratio}$$
#infosys303example if the overcommit ratio is 6, the previous example would advise a number of $8\times 6=48\ VMs\ per\ server$ (splitting workload across 48VMs)

However, Microsoft advises: "Virtual machines possible per server" can vary based on upon the workload the virtual machines are running, the capacity of the server hardware, the requirements of the guest operating system & the efficiency of the [[Hypervisors (Virtual Machine Monitor - VMM)]] & available storage
![[Pasted image 20240521212539.png]]
- Cloud providers are in a sense a capacity planning planner

### [[Memory]]
A typical Windows 7 64-bit enterprise deployment requires 2 vCPUs & 4GB RAM
The native OS alone is approximately 400MB
## Goal
to allocate enough [[Memory]] to hold the set of applications & data while keeping the [[Memory]] [[overcommit ratio]] as low as possible
- this prevents Windows from writing data to the paging file because there is not enough RAM available in the guest OS

[[Memory]] should not be oversubscribed in a [[Virtual Desktop Infrastructure (VDI)]] deployment
### Storage
The Windows 7 64-bit version requires an additional 4GB of disk space over the Windows 7 32-bit version.
- this will decrease the number of virtual machines on the server - unless additional