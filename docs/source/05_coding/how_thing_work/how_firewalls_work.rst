How Firewalls Work
===================================

If you have been using the Internet for any length of time, and especially if you work at a larger company and browse the Web while you are at work, you have probably heard the term firewall used. For example, you often hear people in companies say things like, "I can't use that site because they won't let it through the firewall."

If you have a fast Internet connection into your home (either a DSL connection or a cable modem), you may have found yourself hearing about firewalls for your home network as well. It turns out that a small home network has many of the same security issues that a large corporate network does. You can use a firewall to protect your home network and family from offensive Web sites and potential hackers.

Basically, a firewall is a barrier to keep destructive forces away from your property. In fact, that's why its called a firewall. Its job is similar to a physical firewall that keeps a fire from spreading from one area to the next. As you read through this article, you will learn more about firewalls, how they work and what kinds of threats they can protect you from.

**What is a firewall?**

A firewall is a computer network security system that restricts internet traffic in to, out of, or within a private network.
This software or dedicated hardware-software unit functions by selectively blocking or allowing data packets. It is typically intended to help prevent malicious activity and to prevent anyone—inside or outside a private network—from engaging in unauthorized web activities.

Firewalls can be viewed as gated borders or gateways that manage the travel of permitted and prohibited web activity in a private network. The term comes from the concept of physical walls being barriers to slow the spread of fire until emergency services can extinguish it. By comparison, network security firewalls are for web traffic management — typically intended to slow the spread of web threats.

Firewalls create 'choke points' to funnel web traffic, at which they are then reviewed on a set of programmed parameters and acted upon accordingly. Some firewalls also track the traffic and connections in audit logs to reference what has been allowed or blocked.

Firewalls are typically used to gate the borders of a private network or its host devices. As such, firewalls are one security tool in the broader category of user access control. These barriers are typically set up in two locations — on dedicated computers on the network or the user computers and other endpoints themselves (hosts).

**How do firewalls work?**

A firewall decides which network traffic is allowed to pass through and which traffic is deemed dangerous. Essentially, it works by filtering out the good from the bad, or the trusted from the untrusted. However, before we go into detail, it helps to understand the structure of web-based networks.

Firewalls are intended to secure private networks and the endpoint devices within them, known as network hosts. Network hosts are devices that ‘talk’ with other hosts on the network. They send and receive between internal networks, as well as outbound and inbound between external networks.

Computers and other endpoint devices use networks to access the internet and each other. However, the internet is segmented into sub-networks or 'subnets' for security and privacy. The basic subnet segments are as follows:

- External public networks typically refer to the public/global internet or various extranets.
- Internal private network defines a home network, corporate intranets, and other ‘closed’ networks.
- Perimeter networks detail border networks made of bastion hosts — computer hosts dedicated with hardened security that are- ready to endure an external attack. As a secured buffer between internal and external networks, these can also be used to- house any external-facing services provided by the internal network (i.e., servers for web, mail, FTP, VoIP, etc.). These- are more secure than external networks but less secure than internal. These are not always present in simpler networks like- home networks but may often be used in organizational or national intranets.

Screening routers are specialized gateway computers placed on a network to segment it. They are known as house firewalls on the network-level. The two most common segment models are the screened host firewall and the screened subnet firewall:

- Screened host firewalls use a single screening router between the external and internal networks. These networks are the two subnets of this model.
- Screened subnet firewalls use two screening routers— one known as an access router between the external and perimeter network, and another known as the choke router between the perimeter and internal network. This creates three subnets, respectively.

Both the network perimeter and host machines themselves can house a firewall. To do this, it is placed between a single computer and its connection to a private network.

- Network firewalls involve the application of one or more firewalls between external networks and internal private networks. These regulate inbound and outbound network traffic, separating external public networks—like the global internet—from internal networks like home Wi-Fi networks, enterprise intranets, or national intranets. Network firewalls may come in the form of any of the following appliance types: dedicated hardware, software, and virtual.
- Host firewalls or 'software firewalls' involve the use of firewalls on individual user devices and other private network endpoints as a barrier between devices within the network. These devices, or hosts, receive customized regulation of traffic to and from specific computer applications. Host firewalls may run on local devices as an operating system service or an endpoint security application. Host firewalls can also dive deeper into web traffic, filtering based on HTTP and other networking protocols, allowing the management of what content arrives at your machine, rather than just where it comes from.

A network firewall requires configuration against a broad scope of connections, whereas a host firewall can be tailored to fit each machine's needs. However, host firewalls require more effort to customize, meaning that network-based are ideal for a sweeping control solution. But the use of both firewalls in both locations simultaneously is ideal for a multi-layer security system.

Filtering traffic via a firewall makes use of pre-set or dynamically learned rules for allowing and denying attempted connections. These rules are how a firewall regulates the flow of web traffic through your private network and private computer devices. Regardless of type, all firewalls may filter by some combination of the following:

- Source: Where an attempted connection is being made from.
- Destination: Where an attempted connection is intended to go.
- Contents: What an attempted connection is trying to send.
- Packet protocols: What ‘language’ an attempted connection is speaking to carry its message. Among the networking protocols that hosts use to ‘talk’ with each other, TCP/IP protocols are primarily used to communicate across the internet and within intranet/sub-networks.
- Application protocols: Common protocols include HTTP, Telnet, FTP, DNS, and SSH.

Source and destination are communicated by internet protocol (IP) addresses and ports. IP addresses are unique device names for each host. Ports are a sub-level of any given source and destination host device, similar to office rooms within a larger building. Ports are typically assigned specific purposes, so certain protocols and IP addresses using uncommon ports or disabled ports can be a concern.
By using these identifiers, a firewall can decide if a data packet attempting a connection is to be discarded—silently or with an error reply to the sender-or forwarded.

**Types of firewall**

Different types of firewalls incorporate varied methods of filtering. While each type was developed to surpass previous generations of firewalls, much of the core technology has passed between generations.
Firewall types are distinguished by their approach to:

- Connection tracking
- Filtering rules
- Audit logs

Each type operates at a different level of the standardized communications model, the Open Systems Interconnection model (OSI). This model gives a better visual of how each firewall interacts with connections.
