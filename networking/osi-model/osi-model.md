# osi model

## what is the osi model?

- osi = open systems interconnection
- framework used to explain how devices communicate over a network
- provides a standard that allows different devices and technologies to communicate with each other
- helps organize networking into layers with specific responsibilities

## purpose of the osi model

- standardizes network communication
- allows different devices to understand data sent across a network
- breaks networking into smaller, easier-to-understand parts

## 7 layers of the osi model

7. application
6. presentation
5. session
4. transport
3. network
2. data link
1. physical

## encapsulation

- as data moves through the osi layers, information is added to it
- this process is called encapsulation
- each layer adds information needed for communication

## package delivery analogy

imagine you want to mail a package to a friend.

### layer 7 - application

- decide what message to send
- write the letter

### layer 6 - presentation

- format, translate, compress, or encrypt the message

### layer 5 - session

- start and maintain the conversation

### layer 4 - transport

- ensure the package arrives correctly
- tracking number and delivery confirmation

### layer 3 - network

- determine the route to the destination
- choose which roads and cities to travel through

### layer 2 - data link

- move the package between nearby locations
- local post office to local post office

### layer 1 - physical

- physically transport the package
- trucks, roads, airplanes, and mail carriers

## relating the osi model to networking concepts

### layer 3 - network

- ip addresses
- routers

### layer 2 - data link

- mac addresses
- switches
- arp

### layer 1 - physical

- ethernet cables
- wifi signals

## important notes

- layer 7 is the highest layer (closest to the user)
- layer 1 is the lowest layer (physical cables and signals)
- each layer has its own responsibilities
- data travels through multiple layers before reaching its destination

## key takeaway

- the osi model divides networking into 7 layers
- each layer performs a specific job
- encapsulation adds information as data moves through the layers
- layer 3 deals with ip addresses and routing
- layer 2 deals with mac addresses and local delivery
- layer 1 deals with physical transmission of data
