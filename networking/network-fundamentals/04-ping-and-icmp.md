
#### what is ping
* ping is a network tool used to test communication between devices
* checks whether another device can be reached
* measures how long it takes for data to travel there and back
##### what does ping use
* ping uses icmp (internet control message protocol)
- specifically:
    - icmp echo request
    - icmp echo reply

#### how ping works
##### step 1
your device sends an icmp echo request
"are you there?"
##### step 2
the target device receives the request
##### step 3
the target sends an icmp echo reply
"yes, i'm here."
##### step 4
your device measures how long the round trip took


#### ttl (time to live)
- a counter attached to every packet
- decreases by 1 each time the packet passes through a router
- prevents packets from traveling forever due to routing errors or loops
- when ttl reaches 0, the packet is discarded
***example***
- packet starts with ttl = 64
***path***
* pc → router 1 → router 2 → router 3 → server 
***ttl values***
- 64 → 63 → 62 → 61
##### why ttl exists
sometimes routers can accidentally create loops.
***example:***
router a → router b  
↑ ↓  
router d ← router c
***without ttl:***
- packet could travel forever
- wastes bandwidth
- slows down networks
***with ttl:***
- packet eventually reaches ttl = 0
- packet is discarded
- loop stops
###### analogy
imagine mailing a package with 64 stamps.
- every post office removes one stamp
- when no stamps remain, the package is thrown away

#### different types of pings
##### pinging local router
example:
- ping 192.168.1.254 (usually the default gateway/router)
- tests communication inside the local network
- confirms:
    - device is connected to the network
    - router is reachable
###### analogy:
- knocking on your front door to make sure your house is there
##### pinging a public server
example:
- ping 8.8.8.8 (google's public dns server)
- tests communication with the internet
- confirms:
    - router is working
    - isp is working
    - internet connection is working
###### analogy:
- mailing a letter across the country to make sure you can reach the outside world

##### troubleshooting
***if:***
- ping 192.168.1.254 works
- ping 8.8.8.8 fails
***then:***
- local network is working
- problem is between your router and the internet
