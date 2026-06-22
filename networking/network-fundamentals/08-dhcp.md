#### *dhcp*
dynamic host configuration protocol
- dhcp automatically assigned ip addresses to devices
- prevents you from having to manually configure a device
- usually runs on your router at home

#### why do we need dhcp?
without dhcp:
- every device would need a manually assigned ip address
- easy to make mistakes
- could accidentally assign the same ip address twice
with dhcp:
- devices automatically receive available ip addresses
- reduces configuration errors

#### dhcp process (dora)
dora:
- discover
- offer
- request
- acknowledge
##### 1. dhcp discover
new device joins the network and asks:
- "is there a dhcp server out there that can give me an ip address?"
##### 2. dhcp offer
dhcp server responds:
- "yes, you can use 192.168.1.10"
##### 3. dhcp request
device responds:
- "sounds good, i'd like to use 192.168.1.10"
##### 4. dhcp ack (acknowledgement) 
dhcp server confirms:
- "approved. you may use 192.168.1.10"
device can now communicate on the network.
#### dhcp lease
- temporary permission to use an ip address
- after a period of time, the device renews the lease
