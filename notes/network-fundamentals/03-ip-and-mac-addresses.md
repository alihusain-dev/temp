# ip and mac addresses

## device identification

devices have two ways of being identified:

### ip address

- identifies where a device is on a network
- can change over time

**analogy:**
- your home address

### mac address

- identifies the physical device
- usually permanent
- assigned by the manufacturer

**analogy:**
- your fingerprint

## ip addresses

- used to identify a device on a network
- devices use ip addresses to find and communicate with each other
- no two devices on the same network can have the same ip address at the same time
- ipv4 addresses are made up of 4 octets

### example

- 192.168.1.1

**octets (0-255):**
- 192
- 168
- 1
- 1

## public vs private ip addresses

### private ip address

- used inside a local network
- not directly visible on the internet

**examples:**
- 192.168.1.77
- 192.168.1.74

**analogy:**
- apartment number inside a building

### public ip address

- used to identify your network on the internet
- assigned by your isp (internet service provider)
- multiple devices can share the same public ip address

**example:**
- 86.157.52.21

**example network:**
- laptop = 192.168.1.77
- phone = 192.168.1.74

both appear to the internet as:

- 86.157.52.21

**house analogy:**

- public ip = house address
- private ip = room number

**internet knows:**
- the house address

**router knows:**
- which room to deliver information to

## ipv4

- current common addressing system
- uses 32 bits
- supports about 4.29 billion addresses

### problem

- running out of available addresses due to the large number of connected devices

## ipv6

- newer version of ip addressing
- supports vastly more addresses

### benefits

- solves ipv4 address shortage
- more efficient addressing

### example

- 2a00:22c4:a531:c500:425f:cce6:c36b

## mac addresses

- media access control address
- unique identifier assigned to a network interface
- usually burned into the device by the manufacturer

### example

- a4:c3:f0:85:ac:2d

### structure

**first half:**
- manufacturer/vendor

**second half:**
- unique device identifier

**analogy:**
- serial number of a bag

## spoofing

### mac spoofing

- changing or faking a mac address
- device pretends to have a different identity

### ip spoofing

- faking the source ip address in packets
- makes traffic appear to come from a different device or location

## key takeaway

- ip address = location
- mac address = identity
- private ips are used inside local networks
- public ips identify networks on the internet
- ipv6 was created to solve ipv4 address exhaustion
- mac and ip addresses can both be spoofed
