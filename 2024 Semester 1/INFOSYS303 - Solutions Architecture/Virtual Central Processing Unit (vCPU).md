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
