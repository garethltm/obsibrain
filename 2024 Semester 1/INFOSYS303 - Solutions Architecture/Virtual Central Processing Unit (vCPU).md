- represents a share of a physical Central Processing Unit (CPU) that is assigned to a virtual machine

As it relates to [[virtualization]] & the cloud, multiple [[Virtual Central Processing Unit (vCPU)]] can be assigned to & utilize one [[CPU core]]
## Concepts about virtual servers
1. [[Hypervisors (Virtual Machine Monitor - VMM)]]
2. [[Socket]]
3. [[thread(s)]]
4. [[Physical Core]]
5. [[Logical Core]]
## How many vCPUs?
- a big question for [[Technical Architect (TA)]]

Take the number of processing [[thread(s)]] that a chipset offers per core & multiply the number of occupied [[Socket]]:

$$(Threads \times \ Cores)\times \#Physical\ CPU = NUMBER\ vCPU$$
#infosys303example First, we need to select a virtual server & CPU. For this example, Intel Xeon E-2288G as the underlying CPU. 
An Intel Xeon E-2288G includes:
1. 8 cores
2. 16 threads 
with a 3.7GHz base clock & 5.0GHz turbo boost
$$(16\ Threads\times \ 8\ Cores)\times 1\ CPU = 128\ vCPU$$
## Workload & Utilization
We need to know our workload & application profiles
##### Questions worth considering:
- Do our apps run at 100% CPU utilization all of the time?
	- (what is the expected load, 0-100%)
- Do they have periods where the utilization bursts?
- Do they have maintenance windows?
Theoretically, if we have small VMs that barely use any CPU time, we could easily get 20-30 VMs from an 8-core server

However, if we have larger workloads such as a database server, we will have far fewer VMs from that same 8-core server

At the end, it being good at estimating how many vCPUs per VM:
![[Pasted image 20240509233233.png]]
## How to determine Cloud Server Requirements?
Let's assume a brand-new application that is not running on a server. It has to be built locally on a machine