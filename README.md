# ICS_Project_Group7

## Instruction
 - Read the WEb (1).pdf (presentation slide)
 - watch this video carefully : https://www.youtube.com/watch?v=kUQqTk3SOq8
 - Read the Question bank.
 - Slide Link : https://www.canva.com/design/DAGR1Zb3P4E/BZFX_bPtc5tb6mYZWYiNTA/view?utm_content=DAGR1Zb3P4E&utm_campaign=designshare&utm_medium=link&utm_source=editor
 - arp spoof detection:
   - XArp : https://www.youtube.com/watch?v=LqU5Z5c7JGM
   - wireshark : https://www.youtube.com/watch?v=vsBK_7DEcss
# Evaluation Parts
1) Introduction (ARP, ARP Poisoning, attack surface, attack vulnerabilities and attack anatomy)

2) Demonstration (bettercap application)

3) Attack score (Attack Tree, Common Vulnerability Scoring System)

4) Prevention and Detection (HTTPS, VPN)

## Demonstration Step by Step Command explanation

### Without using a caplet
- `ifconfig` : to find the interface of you network `wlo1` in my case.
- `bettercap -iface wlo1`  This command launches Bettercap, a network monitoring and attack tool.
  - **bettercap**: Starts the Bettercap application.
  - **-iface wlo1**: Specifies the network interface (in this case, `wlo1` for wireless) to use for capturing traffic.
- `net.probe on`  This command enables network probing in Bettercap.

  - **net.probe**: This module scans the network for live hosts and devices.
  - **on**: Activates the probing feature.


- `set arp.spoof.fullduplex true` This command configures Bettercap to enable full-duplex ARP spoofing.
  - **set**: Command used to configure options in Bettercap.
  - **arp.spoof.fullduplex**: The specific option for ARP spoofing behavior.
  - **true**: Activates full-duplex mode, allowing the attacker to intercept and manipulate traffic in both directions between two hosts.

- using `net.show` you can check the victim's IP address. It will give a table in which one column has IP address and other column has mac address and some other informations in other columns.

- `set arp.spoof.targets [Victim's IP address]` This command configures the ARP spoofing target in a tool like Bettercap.

  - **set**: Command used to configure options in Bettercap.
  - **arp.spoof.targets**: The specific option to define which IP address will be the target of the ARP spoofing attack.
  - **[Victim's IP address]**: Placeholder for the actual IP address of the device you want to spoof or target.

- `arp.spoof on` This command enables ARP spoofing in a tool like Bettercap.

  - **arp.spoof**: The feature responsible for ARP spoofing, which tricks devices on the network by sending fake ARP responses.
  - **on**: Activates ARP spoofing, allowing the attacker to begin sending spoofed ARP messages on the network.


- `set net.sniff.local true` **{Optional}** This command configures Bettercap to enable packet sniffing on the local machine.
  - **set**: Command used to configure options in Bettercap.
  - **net.sniff.local**: Option to specify whether to capture local network traffic.
  - **true**: Enables packet sniffing on the local machine, allowing the attacker to capture and inspect traffic generated by the machine running Bettercap.

- `net.sniff on` This command enables packet sniffing in Bettercap.

  - **net.sniff**: The feature responsible for capturing and analyzing network traffic.
  - **on**: Activates packet sniffing, allowing the attacker to monitor and capture all network packets passing through the interface.


**Now if victim login on website which is not secure then the username and password will appeare on you screen.**

### With using a caplet

- `bettercap -iface wlo1 -caplet spoof.cap`
