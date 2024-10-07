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
- An attack surface is the total number of possible points of entry for an unauthorized user to access a system and extract data.
- Vulnerability can refer to a state of being exposed to harm or attack, or to a weakness in a system that can be exploited.
- The anatomy of an attack is a breakdown of the stages and tactics used in a cyberattack.
[![](https://mermaid.ink/img/pako:eNpllE9vm0AQxb_Kas-2ZbAJKYdKMY7aHKpasU9d-zCGgaDCLl0GxU6U794xrP-QcAL2t7Nv3jx4l4lJUUYyt1C_iM1yqwVfD-rheSXWtTFZoXORGStiiylqKqAUMdTUWtw5VozH38VCrSzWYIEKowcrsXo8YNJ-eb9UNyUfD2QhcUxPLfq6nnrSDUFZigUSoU2g3g0AX_0AekErCGyOJArNcqtbHQvfkaCeugOz4xl-Wn1m9lcmB8JXON5APTNzvaJodJF1DpExZXOmZg4DFRudFTl7dRXfmflzs1ldNl86jnu_PLVmdfSlX7fs31Q9Tak5TUlUJm3L80hi36Gg1txk3-vntX235nocHjFTjxr2JXLnJ7mvYNNe5w0zdyrZ-quMkxVABMnfMzx3NKjnVguw9aQDh7UCnnHBOSAUNe9lWckgYnHgOHCHaqRJZ99nYH9jjqshsqJkH5vO-NLkhRYpEFxcX_Zp9NQvwyKYcftSwZHkASW7Aedf89EX436xqqkZYmxhH2mRXFJ-QWaOAbUC22Afh9Xv9UZY_NdiQ1_IvXrQUB7fuKsSwY4JDyRqa8gkffDkSFbIsS9S_pjfT7u3kkdT4VZGfJtiBm1JW7nVH4xCS2Z91ImMyLY4kta0-YuMMtbIT23NBuGyAP4pVJe3Neg_xlTnLfwoo3d5kNHYm_qT6d106gfzb17ozcORPMrIvw8m4WwWhmFwF4R34fxjJN-6At7E96anK_DngT-9v__4Dwa8aKg?type=png)](https://mermaid.live/edit#pako:eNpllE9vm0AQxb_Kas-2ZbAJKYdKMY7aHKpasU9d-zCGgaDCLl0GxU6U794xrP-QcAL2t7Nv3jx4l4lJUUYyt1C_iM1yqwVfD-rheSXWtTFZoXORGStiiylqKqAUMdTUWtw5VozH38VCrSzWYIEKowcrsXo8YNJ-eb9UNyUfD2QhcUxPLfq6nnrSDUFZigUSoU2g3g0AX_0AekErCGyOJArNcqtbHQvfkaCeugOz4xl-Wn1m9lcmB8JXON5APTNzvaJodJF1DpExZXOmZg4DFRudFTl7dRXfmflzs1ldNl86jnu_PLVmdfSlX7fs31Q9Tak5TUlUJm3L80hi36Gg1txk3-vntX235nocHjFTjxr2JXLnJ7mvYNNe5w0zdyrZ-quMkxVABMnfMzx3NKjnVguw9aQDh7UCnnHBOSAUNe9lWckgYnHgOHCHaqRJZ99nYH9jjqshsqJkH5vO-NLkhRYpEFxcX_Zp9NQvwyKYcftSwZHkASW7Aedf89EX436xqqkZYmxhH2mRXFJ-QWaOAbUC22Afh9Xv9UZY_NdiQ1_IvXrQUB7fuKsSwY4JDyRqa8gkffDkSFbIsS9S_pjfT7u3kkdT4VZGfJtiBm1JW7nVH4xCS2Z91ImMyLY4kta0-YuMMtbIT23NBuGyAP4pVJe3Neg_xlTnLfwoo3d5kNHYm_qT6d106gfzb17ozcORPMrIvw8m4WwWhmFwF4R34fxjJN-6At7E96anK_DngT-9v__4Dwa8aKg)
