# 1. Introduction to Computer Network
## A. Data Communications
### Definition
Data communication is the exchange of data between two devices via some form of transmission medium such as wire cable or wireless

For communications to occur, the communicating devices must be part of a communication system made up of a combination of hardware and software

The effectiveness of data communications depends on:
1. Delivery
2. Accuracy
3. Timeliness
4. Jitter

### Components
The message is the information (data) to be communicated. Popular forms of data include text, numbers, audio, and video

The sender is the device that sends the data message. It can be a computer, a telephone handset, a camera, and others

The receiver is the device that receives the message

The transmission medium is the physical path by which a message travels from sender to receiver

A protocol is a set of rules that govern data communication

### Data Flow
1. Simplex
2. Half-duplex
3. Full-duplex

## B. Networks
### Definition
A network is the interconnection of a set of devices capable of communication

A device can be a host, such as a PC, laptop, workstation, cellphone, or security system

A device in this definition can also be a connection device such as a router that connects the network to other networks, a switch that connects devices together, or a modem (modulator-demodulator) that changes the form of data

### Physical Structures
Type of connection
- Point to Point -> single transmitter and receiver
- Multipoint -> multiple recipients of a single transmission

Physical Topology
- Connection of devices
- The topology of a network
  1. Mesh
  2. Star
  3. Bus
  4. Ring

### Categories of Network
1. Local Area Network (LAN)
2. Wide Area Newtwork (WAN)
3. Metropolitan Area Network (MANs)

## The Internet
The internet today is an internetwork that allows any user to become a part of it. The user needs to be connected to an ISP

The physical connection is normally done through a point-to-point WAN such as
- Telephone network
- Cable network
- Wireless network
- Others

## Protocol Layering
### TCP/IP protocol Suite
TCP/IP protocol suite used in the internet today. It is a hierarchical protocol made up of interactive modules, each of which provides a specific functionality. TCP/IP protocol is defined as five layers

| Application |

| Transport   |

| Network     |

| Data Link   |

| Physical    |

### OSI Model
International Organization for Standardization (ISO) makes OSI model

OSI model is a layered framework for the design of network systems that allows communication between all types of computer systems.

# 2. Physical & Data Link
## Transmission Media
### Classification of Transmission Media
1. Bounded/Guided Media
   - Copper cables such as twisted pair and coaxial cable
   - Optical cable
      - Single Mode
      - Multi-Mode
          - Step Index
          - Graded Index
2. Unbounded/Unguided
   - Electromagnetic Wave (VHF, UHF, Microwave)

### Transmission characteristic
- Characteristic and data transmission is determined by the medium used and signal quality
- Data transmission using guided media, the medium itself determines the bandwidth of the communication channel capacity
- Data transmission using electromagnetic waves the bandwidth antenna is important
- Key performance is the transmission data rate and covered distance

## Link Layer Addressing
### Media Access Control (MAC)
Shared-media broadcast technology

Ethernet's MAC performs three function
1. Transmitting and receiving data packets
2. Decoding data packets and checking them for valid addresses before passing them into the upper layers
3. Detecting errors within data packets or on the network

Use Contention Transmission Principle (First Come, First Serve)

Dictates who can transmit and when (Only one station may transmit at a time, otherwise, their signals would be scrambled)

Assembly of data into frame with address and error detection fields

Disassembly of frame
- address recognition
- error recognition

Govern access to transmission medium which is not found in traditional layer 2 data link control

For the same LLC, several MAC options may be available

### Ethernet
Most popular LAN standards

Simple and relatively inexpensive

Scalable - 10 Mbps, 100 Mbps, 1 Gbps

### Logical Link Control (LLC)
Interface to higher-level

Flow and error control

Transmission of link-level PDUs between two stations

Must support multiaccess, shared medium

Relieved of some link access details by MAC layer

# 3. Network Layer - Data Transfer



# 4. IP Addressing
## Class of IP
Classful Addressing

| Class   | Starting Range | Ending Range    |
|---------|----------------|-----------------|
| Class A | 0.0.0.0        | 127.255.255.255 |
| Class B | 128.0.0.0      | 191.255.255.255 |
| Class C | 192.0.0.0      | 223.255.255.255 |
| Class D | 224.0.0.0      | 239.255.255.255 |
| Class E | 240.0.0.0      | 255.255.255.255 |

## Type of IP Address
1. Private IP address (Used for LAN)
2. Public IP address (Used for WAN / Internet)
3. NAT (Translate a Private IP Address to a Public IP Address, typically implemented in routers)
4. Devices (Router is a device that connects two networks, Modem (modulator-demodulator) is a device that translates one type of signal to another type of signal (fiber optic from ISP to home router))

## Uses of IP Addressing
### Network Address
Network addressing is used for routing packets to its destination network

Source IP: 167.199.170.82/24 - Calculated Network Address: 167.199.170.0

Source IP: 167.199.179.82/24 - Calculated Network Address: 167.199.179.0

Network Address source is different from Network Address destination, to forward packet from source to destination, we will use Router

Router will forward packet to other network addresses using Routing Table (Forwarding Table) via interface number

### Broadcast Address

Broadcasting means one-to-all communication. A frame with a destination broadcast address is sent to all entities in the link

The broadcast address is always the highest number possible in a network or sub-network or sub-network

Some protocols used broadcast addresses to send frane to all entities like ARP, RIP, etc

# 5. Subnetting
Designing subnetting 

The subnetwork in a network should be carefully designed to enable the routing of packets. We assume the total number of addresses granted to the organization is N, the prefix length is n, the assigned number of addresses to each subnet is Nsub, and the prefix length of each subnetwork is nsub

Then the following steps need to be carefully followed to guarantee the proper operation of the subnetwork
1. The number of addresses in each subnetwork should be the power of 2
2. The prefix length of each subnetwork should be found using the formula: nsub = 32 - log2Nsub
3. The starting address in each subnetwork should be divisible by the number of addresses in that subnetwork. This can be achieved if we first assign addresses to larger subnetwork

Example:

An organization is granted a block of addresses with the beginning address 14.24.74.0/24. the organization needs to have three subblocks of addresses to use in its three subnets: One subblock of 10 addresses, one subblock of 60 addresses, and one subblock of 120 addresses. design the subblock

# 6. Cloud Computing
## Definition
What is cloud computing?

Cloud computing is the on-demand delivery of IT resources over the Internet with pay-as-you-go pricing

Instead of buying, owning, and maintaining physical data centers and servers, you can access technology services, such as computing power, storage, and databases, on an as-needed basis from a cloud provider such as Amazon Web Service (AWS).

Who is using cloud computing?

Organizations of every type, size, and industry are using the cloud for a wide variety of use cases, such as data backup, disaster recovery, email, virtual desktop, software development and testing, big data analytics, and customer-facing web applications

For example, financial services companies are using the cloud to power real-time fraud detection and prevention, and video game makers are using the cloud to deliver online games to millions of players around the world.

## Benefits of Cloud Computing
1. Agility

   The cloud gives you access to a broad range of techs so that you can innovate faster and build nearly anything that you can imagine
2. Elasticity

   With cloud computing, you don't have to over-provision resources upfront to handle peak levels of business activity. Instead, you provision the amount of resources that you actually need
3. Cost Saving

   The cloud allows you to trade capital expenses (such as data centers and physical servers) for variable expenses, and only pay for it as you use it
4. Deploy globally in minutes
   With the cloud, you can expand to new geographic regions and deploy globally in minutes

## Types of Cloud Computing
1. Infrastructure as a Service (IaaS)

   IaaS contains the basic building blocks for cloud IT. It provides access to networking features, computers, and data storage space.
2. Platform as a Service (PaaS)

   PaaS removes the need for you to manage underlying infrastructure (usually hardware and operating system), and allows you to focus on the deployment and management of your applications

3. Software as a Service (SaaS)

   SaaS provides you with a complete product that is run and managed by the service provider. In most cases, people referring to SaaS are referring to end-user applications (such as web-based email)












































