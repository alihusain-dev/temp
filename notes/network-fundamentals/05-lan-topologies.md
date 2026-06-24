# lan topologies and networking devices

## topology

the layout or design of a network.

## types of topology

### star topology

- all devices connect to a central switch or router
- each device has its own separate connection
- efficient and scalable
- if the central device fails, all communication stops

### bus topology

- all devices share one backbone cable
- inexpensive because less cabling and hardware are required
- bottlenecks occur because every device shares the same path
- if the backbone cable breaks, the entire network fails

### ring topology

- devices form a loop
- data travels around the ring from device to device
- if one cable or device fails, communication for the entire ring can stop

## networking devices

### hub

- sends packets to every device
- devices ignore packets not meant for them
- creates unnecessary traffic

### switch

- smarter than a hub
- remembers which device is connected to which port
- sends packets only to the correct device
- mainly handles local network traffic

#### switch confusion

a switch is not only used when devices communicate with each other.

the switch acts as the entry point into the local network.

even when accessing the internet:

- laptop → switch → router → internet

your device still enters the local network first.

if traffic stays inside the network:

- the switch handles it

if traffic needs to leave the network:

- the switch forwards it to the router
- the router sends it to another network or the internet

### router

- connects different networks together
- routes packets between networks
- sends traffic from your home network to the internet

## local vs non-local traffic

### local traffic

- communication between devices on the same network
- usually handled by a switch

**example:**

- phone → printer

### non-local traffic

- communication with another network or the internet
- handled by a router

**example:**

- phone → youtube server

## network concepts

### scalability

- how easy a network is to expand
- star topology scales well because each device has its own connection to the switch

### bottleneck

- too much traffic sharing one path, causing slowdowns

### redundancy

- backup devices or paths in case something fails

**analogy:**

- having two bridges to a city if one bridge collapses

### home network redundancy

- most home networks have little or no redundancy
- usually only one router and one path to the internet

### business network redundancy

- businesses often have multiple paths and backup equipment
- downtime is much more costly, so reliability is more important

## key takeaway

- topology = the layout of a network
- star, bus, and ring are common network topologies
- hubs send traffic to everyone
- switches send traffic only to the intended device
- routers connect different networks together
- switches handle local traffic
- routers handle non-local traffic
- scalability, bottlenecks, and redundancy affect network performance and reliability
