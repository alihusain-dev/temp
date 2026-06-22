
#### *device identification* 
devices have two ways of being identified:
- ip address = like your name/home address
	- can change
- mac address = like your fingerprint
	- usually permanent 
* mac address identifies the physical device
- ip address identifies where the device is on a network
#### ip addresses:
* used to identify a device on a network
* made up of 4 octets in ipv4
* devices use ip addresses to find and communicate with each other
* no two devices on the same network can have the same ip address at the same time
 ***example:***
- 192.168.1.1
	***octets (0-255):***
		- 192
		- 168
		- 1
		- 1

#### public vs private ip addresses
##### private ip address
* used inside local network
* not visible directly on internet
***examples:***
- 192.168.1.77
- 192.168.1.74
###### analogy:
- apartment number inside a building
##### public ip address
- used to identify your network on the internet
- assigned by your isp (internet service provider)
- multiple devices can share one public ip
	- laptop (192.168.1.77)
	- phone (192.168.1.74)
	- both appear to internet as 86.157.52.21
***example:***
- 86.157.52.21
###### analogy: 
***house:***
- public ip = house address
- private ip = room number
***internet knows:***
- the house address
***router knows:***
- which room to deliver information to

#### ipv4
- current common addressing system
- uses 32 bits
- supports about 4.29 billion addresses
***problem:***
- running out of addresses because there are so many devices

#### ipv6
- newer version of ip addressing
- supports vastly more addresses
***benefits:***
- solves ipv4 address shortage
- more efficient 
***example:***
* 2a00:22c4:a531:c500:425f:cce6:c36b


#### mac addresses
* media access control address
* unique identifier assigned to a network interface
- usually burned into the device by the manufacturer
***example:***
* a4:c3:f0:85:ac:2d
* first half
	* manufacturer/vendor
* second half
	* unique device identifier
###### analogy: 
* serial number of a bag
#### spoofing
##### mac
* changing/faking an address
- device pretends to have a different identity 
##### ip
* fake the source ip address in packets
- pretend the packet came from a different ip (faking location)
