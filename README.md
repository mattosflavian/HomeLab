# My Cybersecurity Home Lab

Welcome to my cybersecurity home lab repository! Here, I'll walk you through my hands-on home lab setup dedicated to cybersecurity experimentation and learning.

## Overview

This home lab is built to simulate a diverse network environment incorporating Windows 10, Windows Server 2019, Kali Linux, and Metasploitable machines interconnected.

## Setup

Router => pfSense Firewall => Physical Host running MacOS => 4 VMs running on Oracle Virtual Box.

### Virtual Machines
- WINDOWS 10 ENTERPRISE - Just grab the Windows 10 Enterprise version for a free trial and use the ISO to create your virtual machine.
  
- WINDOWS SERVER 2019 - Same here. Download an evaluation version of Windows Server.
  
- KALI LINUX - I used Kali as my Linux flavor because it has a ton of cybersecurity-related tools already installed. Feel free to choose your favorite flavor
    
- METASPLOITABLE - It's an essential tool for discovering hidden vulnerabilities using a variety of tools and utilities. Metasploit allows you to enter the mind of a hacker and use the same methods for probing and infiltrating networks and servers.

 ### Configuring ACTIVE DIRECTORY -  Windows Server 2019

  <img width="1804" alt="AD1" src="https://github.com/mattosflavian/HomeLab/assets/22013491/136aa654-056a-45f4-8d2f-f865fdff45a2">

   This is the server manager. Usually, it pops up when you finish installing Windows Server 2019.

<img width="906" alt="2-Select Server Roles" src="https://github.com/mattosflavian/HomeLab/assets/22013491/64741eaa-6631-4a96-a7b4-b35acea47e5a">

   Here I am creating a new server. Click Manage> Add Roles and Features> Choose the ones that are selected in the picture to create a Domain Server and a DNS server.

<img width="911" alt="3- Install" src="https://github.com/mattosflavian/HomeLab/assets/22013491/c4a53074-41fe-49ce-bef3-1e8521920624">

  
   Very straightforward, just click next :)

<img width="918" alt="4-Promote Server" src="https://github.com/mattosflavian/HomeLab/assets/22013491/c221456d-d739-4578-87d8-a40a5ae08f54">

  
   Do not close this page. Click on the link "Promote this server to  a domain controller."

<img width="907" alt="5 - Add New Forest" src="https://github.com/mattosflavian/HomeLab/assets/22013491/8df23188-9e8a-40b0-82f1-423f7f8f1eab">

  
   Choose a domain name, set your password and at the end restart the system!

<img width="911" alt="Screen Shot 2023-12-23 at 8 29 01 PM" src="https://github.com/mattosflavian/HomeLab/assets/22013491/00b21e2b-2ed1-4ccb-aa02-21074832e50a">
  
   And..... tah dahh!! It worked! The SOC/ is my domain and after that is my account as an administrator. When adding more users to this server, their names will be showing here when they try to log in! Now we can add users, set rules, etc.

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

