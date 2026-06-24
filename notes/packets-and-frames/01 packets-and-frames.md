# packets and frames

## what are packets and frames?

- packets and frames are small pieces of data used to send information across a network
- many packets together form a complete message

## packet

- layer 3 (network layer)
- contains ip addressing information (location based)
- used by routers to move data between networks

### packet headers

common information stored in packet headers:

- source ip address
- destination ip address
- ttl (time to live)
- checksum

### key terms

#### ttl (time to live)

- limits how long a packet can travel
- decreases by 1 at each router
- packet is discarded when ttl reaches 0

#### checksum

- used to detect data corruption
- helps verify data integrity

## frame

- layer 2 (data link layer)
- contains mac addressing information (device based)
- used to deliver data on the local network

## encapsulation

- a frame contains a packet
- layer 2 adds mac address information around the packet
- this process is called encapsulation

## analogy

sending a letter:

- packet = the letter
- frame = the envelope

the envelope helps deliver the letter locally, while the letter contains the actual information.

## why packets are used

- large messages are split into smaller pieces
- easier to transmit across networks
- reduces bottlenecks
- allows data to be reassembled at the destination

## key takeaway

- packet = layer 3 = ip addresses
- frame = layer 2 = mac addresses
- frames encapsulate packets
- packets contain headers used for routing and error checking
