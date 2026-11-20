# OSPF Dynamic Routing & Network Configuration

## Objective
Configure a multi-router network using OSPF Area 0 to dynamically exchange routes and enable communication between three LANs.

## Technologies Used
- Cisco Packet Tracer
- Cisco 2911 Routers
- Cisco 2960 Switches
- OSPFv2
- IPv4 Addressing and Subnetting
- Cisco IOS CLI

## Network Design
- 3 routers, 3 switches, and 3 PCs
- Three /24 LAN networks
- Two /30 point-to-point networks
- Single-area OSPF (Area 0)

## Configuration
- Assigned IP addresses to router interfaces and PCs
- Configured OSPF router IDs and network statements
- Configured passive interfaces on user-facing LANs
- Verified OSPF neighbors and learned routes

## Verification
- show ip interface brief
- show ip ospf neighbor
- show ip route
- ping and tracert

## Testing
Successfully verified end-to-end connectivity between all three LANs and tested automatic OSPF route withdrawal and recovery after a link failure.

## Skills Demonstrated
Dynamic routing, OSPF neighbor adjacency, routing table verification, subnetting, Cisco IOS configuration, and network troubleshooting.

## Screenshots
Add topology, neighbor, routing table, connectivity, and failover screenshots here.
