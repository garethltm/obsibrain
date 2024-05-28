- Before server virtualization, every server had a single operating system, typically a single application & connected to 1 or many legacy switch ports.
- Network control & data flow are all managed at an individual switch level.
- Every network component throughout the network infrastructure, from routers to advanced network services like [[Load Balancer(s)]], is locally & individually managed
![[Pasted image 20240528203720.png]]
## 2 major issues are revealed:
1. The control of the network equipment is tied to each device
2. Network equipment capability if fairly inflexible
## Virtual switches provide [[Software Defined Networks (SDN)]] to virtual machines
![[Pasted image 20240528203913.png]]
- Server virtualization was the initial introduction to software defined networking.
- Multiple operating systems can run as virtual machines on a single server
- Each of these virtual machines has [[Software Defined Networks (SDN)]] adapters that connect to a software defined, virtualised network switch
- The [[control plane]] & data planes for these virtual machines are now managed wat the server level on commodity hardware, but the rest of the network remains running traditional hardware.
## Server virtualisation datacentre networking
![[Pasted image 20240528204144.png]]
- Since server virtualisation only provides [[Software Defined Networks (SDN)]] capabilities for the VMs contained on each individual server, the 2 major issues with traditional networking remain:
	1. The control of the network equipment is still tied to each device
	2. Network device capability remains fairly inflexible
## [[Software Defined Networks (SDN)]] for datacentre network infrastructure
![[Pasted image 20240528204328.png]]
- Decrease capit