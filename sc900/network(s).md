is a grouping of interconnected physical components that work together to provide a seamless backbone for all your devices to communicate. The cloud and the internet might seem intangible but even they have physical roots. While there are dozens of parts that help define a network, the ones you're more likely to encounter are: routers, switches, firewalls, access points, and hubs. While most of these are outside the scope of this unit, two are worth calling out.
- The **switch** is the fundamental building block of a modern network. It allows multiple devices to communicate with each other.
- The **router** allows different networks to communicate with each other.
![Diagram that demonstrates how multiple devices connect to a switch, which then connects to the router, which allows access to the Internet.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-network-based-threats-mitigations/media/switch-router.png)
You may have heard of different types of networks, such as wireless networks and local area networks. However, fundamentally, they all fall into one of the following two categories:
- A **private network** is where a level of authentication and authorization is required to access devices and resources, as you might find in your place of work.
- A **public network**, like the internet, is open to any user.
### Connect to your [[network(s)]]
Whatever type of network you're using, there are several different ways that you can connect to it.
- The **Wired** or **Ethernet** connection is still the most common way of connecting to an office network. It requires a physical network cable to connect your computer or laptop to a switch in your network.
- A **Wireless** connection lets your device connect to the network using Wi-Fi. This is typically used at home or in large public venues.
- A **Bluetooth** connection is a short-range device-to-device communication method. Small devices like pedometers, headphones, and smart watches tend to use Bluetooth.
## The client-server topology
![A diagram that shows a simple rendering of the client server with different client devices connecting a central server.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-network-based-threats-mitigations/media/client-server.png)
While [[network(s)]] allow devices or apps to communicate with each other, one of the most common network implementations is the client-server topology. In this model, the client can be one or more devices or applications on a device that wants to do something. The server is responsible for processing each client request and sending back a response.

### How data moves around a [[network(s)]]
A [[network(s)]] exists when you have two or more devices that share data. As you saw in the previous unit, a network is composed of many different physical parts that work together to ensure your data gets to where it's needed. This transmission of data across a network is enabled by a suite of communication protocols, often referred to as TCP/IP. It's named after the two main protocols: 
- [[Transmission Control Protocol (TCP)]]
- [[Internet Protocol (IP)]]

Every network on the planet shares and moves data every second of the day. This data comes in every shape and size, from a simple message to images, and even the movies that are streamed to your home.
1. [[datagram (packet)]]
2. [[IP addresses]]
3. [[Domain Name Service (DNS)]]
4. [[sc900/Routing|Routing]]
## Common threats to network security
- **[[Man-in-the-middle or eavesdropping attack]]**
- **[[Distributed denial of service (DDoS) attack]]**
### Common wireless attacks
Wireless networks allow our devices to seamlessly connect to networks everywhere. In your home, the wireless network allows your smartphone, and always-on IoT devices to connect to the internet. The broad [[availability]] of these networks makes them the perfect target for [[cybercriminal(s)]]. There are many different ways to attack a wireless network:
- **Wardriving** – the term Wardriving was popularized by a couple of 1980s movies. The attacker, typically operating from a vehicle, searches for unsecured wireless networks that have vulnerabilities. Most wardriving attacks seek to use your network for criminal activities, like hacking other computers and stealing personal information.
- **Spoofing Wi-Fi hotspots** – This is similar to a [[Man-in-the-middle or eavesdropping attack]]. The attacker uses their laptop, or a device connected to it, to offer a network access point that mimics a genuine access point. 
	>For example, if you're in a coffee shop looking to access the internet using their guest Wi-Fi, you might see a couple of access points that show the name of the business. One of those could be from a bad actor. If you connect to the bogus access point, anything you do over the network can be intercepted. It also allows the cybercriminal to direct you to bad websites or capture your private data.
- ### Bluetooth attack
	- There has been a growth in Bluetooth devices, from smart watches and audio devices to device-to-device communication. Attacks on Bluetooth networks are less common than for wireless, mostly because the criminal needs to be within range of your device – but it's still a valid [[attack vector(s)]]. 
		- A **Bluejacking** attack is where a criminal sends unsolicited messages to any Bluetooth-enabled device that's within range of their own. Bluejacking is similar to when someone rings your doorbell and then runs away before you can answer. It's mostly an annoyance.