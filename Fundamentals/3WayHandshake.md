# What is a Three-Way Handshake?
Also know as TCP handshake or SYN-SYN-ACK.
A method used in a TCP/IP network used to create a connection between a local host and server.
It is a 3-step method allowing both nodes to negotiate the network parameters before attempting to communicate data.
The handshake creates a TCP socket connection to transmit data between the two devices.

# The Three Steps
## 1. Connection between server and client is established
Target server must have open ports to be able to accept traffic.
The client sends a SYN (Synchronise Sequence Number) packet to the target server.
The SYN packet is a number sequence asking if the server is open for new connections

## 2. Server receives SYN packet and replies
The inital SYN packet arrives and is successfully accepted and read by the server.
It reponds back to the client with a confirmation receipt in the form of a SYN/ACK packet.
The packet is split into two parts.
The first is the ACK (Acknowledgement Sequence Number) and is set to one more than the SYN it received intially (e.g. SYN + 1)
The second is the SYN and is another sequence of numbers.
This step is to acknowledge that the server read the first SYN packet properly and correctly, and is now sending its own packet to be acknowledged correctly.

## 3. Client receives SYN/ACK packet and replies again
Client receives SYN/ACK and sends its own ACK packet in response. Again, it is formed by SYN + 1
Once this step is complete, a connection is created and the two nodes can communicate.
