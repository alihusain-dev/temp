# layer 4 - transport layer

## what is the transport layer?

- responsible for transmitting data between devices
- controls how data is sent and received
- uses different protocols depending on what is needed

## how it works

- data is split into smaller pieces called packets
- packets are sent between devices
- the transport layer decides how reliable the connection needs to be

## key terms

### tcp (transmission control protocol)

- connection-based protocol
- focuses on reliability and accuracy
- makes sure all data arrives correctly
- performs error checking

### how tcp works

- creates a connection between two devices
- sends packets
- checks that packets arrive
- reassembles packets in the correct order

### advantages of tcp

- guarantees accurate data
- confirms packets were received
- reliable for important information

### disadvantages of tcp

- slower because it checks everything
- requires more processing

### examples

- web browsing
- file transfers
- emails

## udp (user datagram protocol)

- connectionless protocol
- focuses on speed
- sends data without confirming it arrived

### advantages of udp

- faster than tcp
- less delay
- good for real-time communication

### disadvantages of udp

- does not guarantee delivery
- packets can be lost

### examples

- video streaming
- gaming
- voice calls

## analogy

delivery truck:
- ensures all packages arrive in the right order
- reassembles them correctly
- if any piece is missing it sends it again

### tcp

- tracked shipping
- confirms delivery
- makes sure every package arrives

### udp

- regular mail
- sends it quickly
- does not check if every piece arrived

## key takeaway

- transport layer controls data delivery
- tcp = reliable but slower
- udp = faster but less reliable
- choose tcp or udp depending on the situation
