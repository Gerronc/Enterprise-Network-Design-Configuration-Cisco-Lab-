# Enterprise-Network-Design-Configuration-Cisco-Lab-

In this project, I designed and implemented a small-scale enterprise network using a Cisco Layer 3 switch, two client machines, and a server. The goal was to simulate real-world network segmentation, routing, and service deployment.

Key Achievements:
	•	Designed a network using multiple VLANs and subnetting to separate clients and services
	•	Configured inter-VLAN routing using SVIs, eliminating the need for a dedicated router
	•	Deployed a DHCP server and configured scopes for multiple VLANs
	•	Implemented DHCP relay using ip helper-address to enable cross-VLAN communication
	•	Performed network testing and validation using ping and IP configuration tools
	•	Analyzed and exported Cisco switch configurations for verification and documentation

Challenges & Solutions:
	•	Resolved DHCP failures by correcting inactive scopes and misconfigured relay addresses
	•	Identified connectivity issues caused by dual network interfaces (WiFi vs LAN conflict) and resolved by isolating the correct interface
	•	Gained experience troubleshooting across multiple layers (server, switch, and client systems)

Skills: Cisco Networking, Putty

<h2>Network Diagram</h2>

<p align="center">
<img src="https://i.imgur.com/H5Tpu0U.png" height="85%" width="85%" alt="Network Diagram"/>
</p>


<h2>Client IP Configuration</h2>

Ipconfig output from Client A showing successful DHCP lease acquisition—IPv4 address 10.3.48.6, subnet mask 255.255.255.240, and default gateway 10.3.48.1. Confirms DHCP is functioning correctly within VLAN 10.


<p align="center">
<img src="https://i.imgur.com/VOCHqD1.png" height="85%" width="85%" alt="Server to client B ping"/>
</p>


<h2>Running Configuration output</h2>
Key excerpts from the Cisco switch 

<p align="center">
<img src="https://i.imgur.com/eus3lad.png" height="85%" width="85%" alt="Running Configuration output"/>
</p>

<h2>Server to client B ping</h2>

<p align="center">
<img src="https://i.imgur.com/QotGDuN.jpeg" height="85%" width="85%" alt="Server to client B ping"/>
</p>
Successful ping from Server (VLAN 30) to Client B (VLAN 20), confirming inter-VLAN routing is operational. The replies demonstrate that SVI routing and DHCP relay are correctly configured.

