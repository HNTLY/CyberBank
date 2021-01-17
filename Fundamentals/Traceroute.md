# Traceroute
## Description
A command that runs tools used for network diagnostics.
These tools trace the paths the data takes when going from its source to destination.
The tool will verify the path your data will take, without actually sending the data.
Network Administrators can use this to map the route data will take.
They can also use it for diagnostics and figure out where there is an issue in the network. 
Traceroute most commonly uses ICMP echo packets.
Windows - tracert
Linux/Mac - traceroute

## How does it work?
Every packet sent has a TTL (Time To Live).
The time is measure in 'hops' which is each jump the packet takes between nodes. 
Once the TTL runs out, the packet is dropped.
Each time the packet reaches a new node, its TTL is reduced by one. 
If a node receives a packet with TTL=1, then it will discard the packet and return the response: `ICMP TTL exceeded messages`

## Example usage

Run a traceroute command to Google's publicy available DNS server
`traceroute -n 8.8.8.8`

![/CyberBank/Images/traceroute.JPG](Traceroute)

This UDP packet includes the following:
    - Source address (Our IP)
    - Destination address (8.8.8.8)
