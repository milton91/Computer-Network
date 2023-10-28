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

  


































