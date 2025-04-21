                  STP with EtherChannel in Cisco Packet Tracer

Project Description:
This project demonstrates how to configure Spanning Tree Protocol (STP) to prevent Layer 2 loops and implement EtherChannel (LACP) between switches for link aggregation and redundancy in a small enterprise network using Cisco Packet Tracer.

Objectives:
•	Simulate an enterprise network topology with multiple redundant paths.
•	Configure EtherChannel (LACP) between switches for bandwidth enhancement.
•	Enable STP to ensure loop-free topology and failover handling.
•	Verify link status and spanning-tree behavior using Cisco CLI.

Network Devices Used:
•	3 Cisco 2960 Switches (SW1, SW2, SW3)
•	2 End Devices (PC1, PC2)
•	Copper Straight-Through Cables

Network Topology:

 


Interface Mapping:
Connection	Device A - Interface	Device B - Interface
PC1 ↔ SW1	PC1 - Fa0 ↔ SW1 - Fa0/5	
PC2 ↔ SW2	PC2 - Fa0 ↔ SW2 - Fa0/5	
SW1 ↔ SW2	Fa0/1, Fa0/2	Fa0/1, Fa0/2
SW1 ↔ SW3	Fa0/3, Fa0/4	Fa0/1, Fa0/2
SW2 ↔ SW3	Fa0/3, Fa0/4	Fa0/3, Fa0/4

Output:
On SW1:
 
 
 

On SW2:
 
 

 
On SW3:
 
 

 

Expected Behavior:
•	One link will be blocked by STP to prevent loops.
•	If an active link fails, STP re-converges and activates the blocked port.
•	EtherChannel combines bandwidth and provides redundancy.

