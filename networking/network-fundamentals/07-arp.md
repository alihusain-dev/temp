# arp (address resolution protocol)

## arp

address resolution protocol.

- used to find a device's mac address when you already know its ip address
- allows devices to identify and communicate with each other on a local network
- only works on a lan (local area network)

## why is arp needed?

devices have two identifiers:

### ip address

- where the device is

### mac address

- who the device is

before sending data to a device, you need its mac address.

arp links:

- ip address ↔ mac address

## arp cache

- every device maintains an arp cache
- stores previously learned ip-to-mac mappings
- prevents devices from repeatedly asking for the same mac address
- speeds up communication

## how arp works

### step 1: arp request

a device sends a message to every device on the network:

> "who has ip address 192.168.1.10?"

- all devices receive the request
- only the correct device responds

### step 2: arp reply

the device that owns the ip address replies:

> "i have ip address 192.168.1.10"

the device also sends back its mac address.

### step 3: store in cache

- the requesting device stores the mapping
- future communication can happen immediately without another arp request

## analogy

arp is essentially asking:

> "what device owns this private ip address?"

imagine you know a person's home address but not their phone number.

you stand in the neighborhood and shout:

> "who lives at 123 oak street?"

everyone hears you, but only the correct person responds:

> "i do!"

now you know:

- home address = ip address
- phone number = mac address

### arp cache analogy

after learning their phone number, you save it in your contacts.

next time you need to contact them:

- you don't ask the neighborhood again
- you already have the number saved

### analogy mapping

- home address = ip address
- phone number = mac address
- asking the neighborhood = arp request
- person replying = arp reply
- contacts list = arp cache

## key takeaway

- arp finds a mac address using a known ip address
- arp only works on local networks
- arp request = "what device owns this ip address?"
- arp reply = device responds with its mac address
- arp cache stores ip-to-mac mappings for future use
