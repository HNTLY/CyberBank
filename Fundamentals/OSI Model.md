# Open Systems Interconnection Model
## Description 
Conceptual and Logical layout to define network communication

## 7 Layers
Layer | Name | Description
-- | -- | --
7 (Top) | Application | Users interact with this layer directly 
6 | Presentation | Translates data for application layer
5 | Session | Controls conversations between computers
4 | Transport | Manages delivery and error checking of packets 
3 | Network | Responsible for packet forwarding
2 | Data Link | Transfers data between nodes on same network
1 (Bottom) | Physical | Physical equipment in data transfer

## Application
Closest layer to end user.

Examples: Chrome, Skype, Word, Outlook etc

## Presentation
Translates data based on syntax for each application. Therefore, sometimes called the syntax layer.

Can also handle encryption/decryption required from the application layer

"Presents" the data for the application layer

Example: Encryption/Decryption of data for secure transmission

## Session
A session is created when two computers need to speak.

Functions include: setup, coordination and termination

Coordination example: How long a computer should wait for a response

Example: SCP (Session Control Protocol)

## Transport
Regulates size, sequencing and transport of data between systems.

Examples: How much data to send, rate of sending, destination etc.

Example protocols: TCP (Transmission Control Protocol), UDP (User Datagram Protocol)

## Network
Selects the best logical path for data transfer between nodes.

Finds destination using logical adresses (e.g IP). 

## Data Link
Takes the packets from the network layer and breaks them up into smaller pieces (frames).

Frames synchronise the information to remove transmission errors.

When the receiver receives a frame, they send an acknowledgement frame back.

## Physical
Examples: cables and switches

Data will also be converted into a bit stream (binary string).

Both the physical layers on each end must agreee on a signal convention (e.g Half Duplex, Full Duplex). This ensures that when a 1 or a 0 is sent, it is still receieved as a 1 or 0.

