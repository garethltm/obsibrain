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

$$(Threads \times \ Cores)$$
