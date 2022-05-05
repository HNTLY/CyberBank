# TCP (Transmission Control Protocol)
Data transportation protocol

Connection-oriented protocol

Provides error checking

Guarantees delivery of data and that packets will be delivered in order

Used when reliability is required over speed e.g HTTP, FTP, SSH

# UDP (User Datagram Protocol)
Data Transportation protocol

Connectionless protocol

Doesn't perform error checking

Continuously sends datagrams to the receiver regardless of if they're received or not

Data can also be received out of order or even not at all

Used when speed is required over usability e.g Media streaming (because some lost frames are fine), some gaming (Don't need every single update), DNS

# ICMP (Internet Control Message Protocol)
Provides different function to TCP and UDP

Control protocol

Carries information about the network itself NOT application data

ICMP is most known for the 'ping' utility
  - ICMP probes remote hosts for responsiveness and round-trip time
