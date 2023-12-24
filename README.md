# My Cybersecurity Home Lab

Welcome to my cybersecurity home lab repository! Here, I'll walk you through my hands-on home lab setup dedicated to cybersecurity experimentation and learning.

## Overview

This home lab is built to simulate a diverse network environment incorporating Windows 10, Windows Server 2019, Kali Linux, and Metasploitable machines interconnected.

## Setup

Router => pfSense Firewall => Physical Host running MacOS => 4 VMs running on Oracle Virtual Box.

### Virtual Machines
- Windows 10
  *Just grab the Windows 10 Enterprise version for a free trial and use the ISO to create your virtual machine.
- Windows Server 2019
  *Same here. Download an evaluation version of Windows Server.
- Kali Linux
  * I used Kali as my Linux flavor because it has a ton of cybersecurity-related tools already installed. Feel free to choose your favorite flavor
- Metasploitable
 * It's an essential tool for discovering hidden vulnerabilities using a variety of tools and utilities. Metasploit allows you to enter the mind of a hacker and use the same methods for probing and infiltrating networks and servers.

 ### Configuring Active Directory Windows Server 2019
<img width="907" alt="5 - Add New Forest" src="https://github.com/mattosflavian/HomeLab/assets/22013491/a2ccafff-931c-4ba5-b87d-29cb46f990c8">
This is the server manager. Usually, it pops up when you finish installing Windows Server 2019.
<img width="918" alt="4-Promote Server" src="https://github.com/mattosflavian/HomeLab/assets/22013491/d1888b3f-142e-41c0-bdab-e6864d831d0e">
Here I am creating a new server. Click Manage> Add Roles and Features> Choose the ones that are selected in the picture to create a Domain Server and a DNS server.
<img width="911" alt="3- Install" src="https://github.com/mattosflavian/HomeLab/assets/22013491/e8b35462-d657-452b-9720-dc25bd9c1113">
Very straight forward, just click next :)
<img width="1804" alt="AD1" src="https://github.com/mattosflavian/HomeLab/assets/22013491/daf8d4ec-900c-4c05-85ec-524d227d7e83">
Do not close this page. Click on the link "Promote this server to  a domain controller."
<img width="906" alt="2-Select Server Roles" src="https://github.com/mattosflavian/HomeLab/assets/22013491/6c07c17a-a4f0-481d-88b4-231369392857">
Choose a domain name, set your password and at the end restart the system!
<img width="911" alt="Screen Shot 2023-12-23 at 8 29 01 PM" src="https://github.com/mattosflavian/HomeLab/assets/22013491/00b21e2b-2ed1-4ccb-aa02-21074832e50a">
And..... tah dahh!! It worked! Now we can add users, set rules, etc.

### Network Configuration
- pfSense Firewall
- VLAN setup for segmentation
- All VMs NETWORK TAB were set to bridge mode.

## Security Measures

Implemented security measures include:
- VLAN segregation for network isolation
- pfSense firewall rules for traffic filtering
- Specific configurations on individual machines for hardening


## Conclusion

This home lab serves as an invaluable platform for honing my cybersecurity skills by practically experimenting with various operating systems, network configurations, and security measures.

For any questions or feedback, reach me at spinkkz@gmail.com

