# dhcp (dynamic host configuration protocol)

## dhcp

dynamic host configuration protocol.

- automatically assigns ip addresses to devices
- prevents you from having to manually configure devices
- usually runs on your home router

## why do we need dhcp?

### without dhcp

- every device would need a manually assigned ip address
- easy to make mistakes
- could accidentally assign the same ip address twice
- more time-consuming to manage

### with dhcp

- devices automatically receive available ip addresses
- reduces configuration errors
- simplifies network management

## dhcp process (dora)

remember:

- discover
- offer
- request
- acknowledge

### 1. dhcp discover

a new device joins the network and asks:

> "is there a dhcp server out there that can give me an ip address?"

### 2. dhcp offer

the dhcp server responds:

> "yes, you can use 192.168.1.10"

### 3. dhcp request

the device responds:

> "sounds good, i'd like to use 192.168.1.10"

### 4. dhcp acknowledge (ack)

the dhcp server confirms:

> "approved. you may use 192.168.1.10"

the device can now communicate on the network.

## dhcp lease

- temporary permission to use an ip address
- after a period of time, the device renews the lease
- prevents ip addresses from being permanently assigned to inactive devices

### example

> "you may use 192.168.1.10 for the next 24 hours"

after the lease expires, the device asks to renew it.

## analogy

imagine checking into a hotel.

### discover

you ask:

> "do you have any rooms available?"

### offer

the front desk replies:

> "yes, room 210 is available."

### request

you respond:

> "great, i'd like room 210."

### acknowledge

the front desk confirms:

> "perfect. room 210 is yours."

### analogy mapping

- hotel room = ip address
- front desk = dhcp server
- guest = device
- hotel stay = dhcp lease

## key takeaway

- dhcp automatically assigns ip addresses
- most home routers act as dhcp servers
- dora = discover → offer → request → acknowledge
- devices receive temporary ip leases
- dhcp prevents ip conflicts and simplifies network management
