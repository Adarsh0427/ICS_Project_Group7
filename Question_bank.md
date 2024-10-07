# Possible Questions

## ARP (Address Resolution Protocol)
 - Protocol used to map IP Address of a machine to its MAC address.
 - Stateless protocol: ARP doesn't use sequence numbers to track the order of packets or ensure delivery. This is protocol's lack of state and authentication
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

# Attack Tree 
[![](https://mermaid.ink/img/pako:eNp1k8uO2jAUhl_F8ppBSQi3LCpxa8uiEiqsalgcnONgTWJbjiNgEO9eTxLopKPJJrb_71ztc6Ncp0gTmlkwJ7Jb7hXx34z9QEcMlOVZ25SASklVol0vD-Tl5RuZsw1aoW1BZr83ZGu0FlJl5CzdiczRObQczKFxNa8tFmzrHVbmC3nJVhfklcOOww6yYgswrrJYZwMK8usbEmdBCMk92bCLJlrI1qp0kOef4rVAxBZaCZm9-1PofJWvRCpPCuD49LZskgvZSsEx7yZHCp1WOR46ZFSX6cBm_rfedMVBLWbg8AzXRm30VVPgM0yppBBouxFaKHo00gB_9SveNKULDdjMmPxKhMx9SSXxV0W4xRSVk5CX_wIPWh7Yz91u86GbHfVYq9uvZM6-d2xbOWoThufFNSmXh_-AI5u1t9kWk5IUHHzwdHyQvkUXH4i7x3P8RERP4vF6D7RHC7QFyNS_89u7xZ66Exa4p4lfpiigyt2e7tXdo1A5vb0qThNnK-xRq6vsRBPh--Z3lfGp4VKCn5fieWpA_dG6eJj4LU1u9EKTQTTuB-EkCIbBKB4Nx6MevdIkHMb9MI6CYBJPwyiehPcefavtg_4wno6icBz482A4mHoDTKXT9lczpvW03v8Cpn4kRQ?type=png)](https://mermaid.live/edit#pako:eNp1k8uO2jAUhl_F8ppBSQi3LCpxa8uiEiqsalgcnONgTWJbjiNgEO9eTxLopKPJJrb_71ztc6Ncp0gTmlkwJ7Jb7hXx34z9QEcMlOVZ25SASklVol0vD-Tl5RuZsw1aoW1BZr83ZGu0FlJl5CzdiczRObQczKFxNa8tFmzrHVbmC3nJVhfklcOOww6yYgswrrJYZwMK8usbEmdBCMk92bCLJlrI1qp0kOef4rVAxBZaCZm9-1PofJWvRCpPCuD49LZskgvZSsEx7yZHCp1WOR46ZFSX6cBm_rfedMVBLWbg8AzXRm30VVPgM0yppBBouxFaKHo00gB_9SveNKULDdjMmPxKhMx9SSXxV0W4xRSVk5CX_wIPWh7Yz91u86GbHfVYq9uvZM6-d2xbOWoThufFNSmXh_-AI5u1t9kWk5IUHHzwdHyQvkUXH4i7x3P8RERP4vF6D7RHC7QFyNS_89u7xZ66Exa4p4lfpiigyt2e7tXdo1A5vb0qThNnK-xRq6vsRBPh--Z3lfGp4VKCn5fieWpA_dG6eJj4LU1u9EKTQTTuB-EkCIbBKB4Nx6MevdIkHMb9MI6CYBJPwyiehPcefavtg_4wno6icBz482A4mHoDTKXT9lczpvW03v8Cpn4kRQ)

## Terms:
- An eavesdropping attack occurs when a hacker intercepts, deletes, or modifies data that is transmitted between two devices.
- An attack surface is the total number of possible points of entry for an unauthorized user to access a system and extract data.
- Vulnerability can refer to a state of being exposed to harm or attack, or to a weakness in a system that can be exploited.
- The anatomy of an attack is a breakdown of the stages and tactics used in a cyberattack.
- Hypertext Transfer Protocol Secure (HTTPS) uses Transport Layer Security (TLS) or Secure Sockets Layer (SSL) to encrypt data between a browser and a server. This encryption is done using public key cryptography, which involves two keys: a public key and a private key.
- TLS and SSL are both protocols that allow secure communication between devices and applications on the internet.
- Stands for Transport Layer Security, and is an upgraded version of SSL that fixes vulnerabilities and authenticates more efficiently.

