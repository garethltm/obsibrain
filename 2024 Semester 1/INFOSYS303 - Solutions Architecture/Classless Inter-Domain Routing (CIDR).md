We use the [[Internet Protocol version 4 (IPv4)]] (& [[Internet Protocol version 6 (IPv6)]]) addresses to allocate them to devices in a network. Laptops, PCs, workstations, wireless devices, servers, router interfaces, all receive each one [[Internet Protocol version 4 (IPv4)]] address, which is used to recognise the origin or the destination of the packets that make up a message or a session.

We call [[Classless Inter-Domain Routing (CIDR)]] the technique that allows us to organise the allocation of IP addresses to the devices in a network.

Typically, what an organisation obtains from the country's Internet authority is a block of addresses. The organisation then proceeds to subdivide the block into as many subblocks as subnetworks exist in the organisation's network

#infosys303example ![[Pasted image 20240414161349.png]]

## Constraints on addresses in a block
Which addresses in a block cannot be used to be allocated to devices in a [[Subnet]]?

When a [[Virtual Private Cloud]] [[Classless Inter-Domain Routing (CIDR)]] block is used, the following addresses cannot be used for devices:
#infosys303example Suppose the assigned block is $10.0.0.0/24$
- None of the 1st 4 addresses, that is, 10.0.0