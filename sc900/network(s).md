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
### The datagram or packet
Networks exist to help make device-to-device or system-to-system communication easier. Whatever the size of data, it all needs to be broken down into tiny, uniform chunks. These chunks are called datagrams but are also more commonly known as packets.

Imagine that you want to stream a movie to your device. Given the enormous size of the data involved, the streaming server can't give you the whole movie in one go. Instead, the movie is broken up into billions of packets. Each packet contains a small part of the movie, which is then sent to your device. Your device has to wait until enough packets have been received before you can start watching the movie. In the background, the server continues to send a steady stream of packets to your device just ahead of what's being displayed. If your network speed slows down, then the packets may not reach you in time. The picture you see might become distorted or blocky and there may be gaps in the sound.