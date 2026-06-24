# subnetting

## subnetting

splitting one large network into smaller networks (subnets).

- helps organize devices
- helps manage traffic
- improves efficiency and security

### analogy

- one cake = one large network
- slices of cake = subnets
- subnetting decides who gets which slice

## why use subnetting?

- improve organization
- improve efficiency
- improve security
- give administrators more control

### example

instead of placing every device on one giant network:

- accounting subnet
- finance subnet
- human resources subnet

## subnet masks

a subnet mask tells us:

- which part of an ip address is the network
- which part is the host/device

### example

**ip address:**

- 192.168.1.100

**subnet mask:**

- 255.255.255.0

**result:**

- 192.168.1 = network
- 100 = host

### why does 255 mean "network"?

subnet masks work in binary.

**examples:**

- 255 = 11111111
  - all 1s = network bits

- 0 = 00000000
  - all 0s = host bits

## binary subnet mask example

**subnet mask:**

- 255.255.255.0

**binary:**

- 11111111.11111111.11111111.00000000

**meaning:**

- network.network.network.host

## counting hosts

to determine how many addresses a subnet can contain:

### formula

- 2^(number of host bits)

### example

**subnet mask:**

- 255.255.255.0

**binary:**

- 11111111.11111111.11111111.00000000

**host bits:**

- 00000000

calculation:

- 2^8 = 256 total addresses
- 256 - 2 = 254 usable addresses

### reserved addresses

two addresses are reserved:

#### network address

- identifies the network itself

#### broadcast address

- used to send a message to every device on the network

## addresses in a subnet

### network address

- identifies the network itself
- represents the start of the network
- tells devices which network they belong to

**example:**

- 192.168.1.0

**analogy:**

- the name of the neighborhood
- "oak street neighborhood"

### host address

- identifies a specific device on the network

**example:**

- 192.168.1.100

**analogy:**

- a specific house in the neighborhood
- "123 oak street"

### default gateway

- device that sends traffic to other networks
- usually the router
- used whenever data needs to leave the local network

**example:**

- 192.168.1.254

**analogy:**

- the neighborhood exit/highway entrance

if you're visiting another neighborhood or city, you leave through the highway entrance first.

### rule

**same network:**

- communicate directly

**different network or internet:**

- send traffic to the default gateway

## key takeaway

- subnetting divides large networks into smaller networks
- subnet masks determine the network and host portions of an ip address
- network address = identifies the network
- host address = identifies a device
- default gateway = sends traffic to other networks
- broadcast address = sends traffic to every device on the subnet
