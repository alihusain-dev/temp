#### *what is arp?* 
arp = address resolution protocol
- used to find device's mac address when you already know it's ip address
- allows devices to identify and communicate with each other on a local network
	- only works on lan

#### why is arp needed?
devices have two identifers: 
- ip address = where the device is
- mac address = who the device is
before sending data to a device, you need it's mac address
arp is the link between ip address ↔ mac address
#### arp cache
- every device has an arp cache
- it stores previously learned ip-to-mac mappings
- prevents the device from having to repeatedly ask for the same mac address
#### how arp works
##### step 1: arp request
a device sends a message to every device on the network:
- "who has the ip address 192.168.1.10"
	- all devices receive the request
	- only trhe correct device responds
##### step 2: arp reply
the device that owns the ip address replies
- "i have the ip address 192.168.1.10"
- sends its mac address back to the device that requested the arp
##### step 3: store in cache
- the requesting device stores the mapping
- future communication can happen immediately without another arp request
##### *analogy*
arp is simply asking:
"what device owns this private ip address?"
- imagine you know a person's home address but not their name.
- you stand in the neighborhood and shout:
	- "who lives at 123 oak street?"
- everyone hears you, but only the correct person responds:
	- "i do!"
- now you know:
	- home address = ip address
	- person's identity = mac address
