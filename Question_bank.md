# Possible Questions

## ARP (Address Resolution Protocol)
 - Protocol used to map IP Address of a machine to its MAC address.
 - Why mapping is important ? 
   - The lengths of the IP and MAC addresses differ, and a translation is needed so that the systems can recognize one another.
   - The most used IP today is IP version 4 (IPv4). An IP address is 32 bits long. However, MAC addresses are 48 bits long.
   - ARP translates the 32-bit address to 48 and vice versa.
 - MAC address ?
   - media access control address (48-bit hexadecimal address) is a unique identifier assigned to a network interface controller (NIC) which is used as a network address in communications within a network segment. 
 - Types of ARP Table:
   - Proxy ARP : Technique to answer ARP request of one network device made by other network device.
   - Gratuitous ARP : Procedure carried out by host on a network to update its IP-to-MAC address.
   - Reverse ARP (RARP) : Used by host machines to discover their own IP address.
   - Inverse ARP (IARP) : IARP uses a MAC address to find an IP address. (note : ARP uses an IP address to find a MAC address).

## ARP Spoofing/ARP Poisoning/ARP cache poisoning
This is a type of malicious attack in which a attacker sends fake ARP messages to a target LAN with the intention of linking 
their MAC address with the IP address of a legitimate device or server within the network. The link allows for data from the 
victim's computer to be sent to the attacker's computer instead of the original destination. 

## Terms:
- An eavesdropping attack occurs when a hacker intercepts, deletes, or modifies data that is transmitted between two devices.
