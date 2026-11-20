# Cisco Networking Labs | Network Engineering Portfolio

Welcome to my networking lab portfolio!

This repository documents my hands-on networking projects developed using **Cisco Packet Tracer and Cisco IOS**. These labs demonstrate practical experience with network design, configuration, routing, switching, VLAN segmentation, IP addressing, access control, and troubleshooting.

I am an IT professional with over six years of enterprise IT support experience, CompTIA Network+ and Security+ certifications, and a B.S. in Computer Networks and Cybersecurity.

I created this portfolio to strengthen my networking skills, document my technical work, and demonstrate my continued professional development as I pursue opportunities in network engineering.

---

## Technical Skills Demonstrated

**Routing & Switching**
- Cisco IOS configuration and troubleshooting
- OSPF dynamic routing
- Static routing and default route advertisement
- Layer 2 and Layer 3 switching
- VLAN configuration and segmentation
- IEEE 802.1Q trunking
- Router-on-a-stick and SVI-based inter-VLAN routing

**Network Security**
- Standard networking segmentation principles
- Extended Access Control Lists (ACLs)
- Source and destination IP filtering
- Traffic restriction between VLANs

**Network Infrastructure**
- IPv4 addressing and VLSM subnetting
- Default gateway configuration
- Router and switch interface configuration
- Routing table analysis
- ICMP connectivity testing
- Network troubleshooting and verification

---

## Networking Projects

### 01. OSPF Dynamic Routing & Network Configuration

**Technologies:** Cisco IOS, OSPF, Dynamic Routing, ASBR, Passive Interfaces

Designed and configured a simulated multi-router network using OSPF to dynamically exchange routing information between routers.

**Key Implementations:**
- Configured router interfaces and loopback interfaces.
- Established OSPF neighbor adjacencies.
- Configured passive interfaces.
- Advertised a default route from an Autonomous System Boundary Router (ASBR).
- Verified OSPF routing tables, route propagation, and end-to-end connectivity.

**Project Folder:** `01-OSPF-Dynamic-Routing`

### 02. VLAN Segmentation, 802.1Q Trunking & Inter-VLAN Routing

**Technologies:** VLANs, Cisco IOS, 802.1Q, Router-on-a-Stick

Configured a segmented network using VLANs and implemented router-on-a-stick routing to enable communication between separate departmental networks.

**Key Implementations:**
- Created VLANs and assigned access ports.
- Configured 802.1Q trunk connections.
- Restricted allowed VLANs and configured a dedicated native VLAN.
- Configured router subinterfaces and default gateways.
- Verified cross-VLAN connectivity.

**Project Folder:** `02-VLAN-Trunking-InterVLAN-Routing`

### 03. VLSM Subnetting & Static Routing

**Technologies:** IPv4, VLSM, Static Routing, Cisco IOS

Designed an IP addressing scheme using Variable Length Subnet Masks (VLSM) to efficiently allocate IP addresses across multiple LANs and a point-to-point WAN connection.

**Key Implementations:**
- Subnetted the 192.168.5.0/24 network based on host requirements.
- Assigned IP addresses to router interfaces and end devices.
- Configured static routes between networks.
- Verified routing tables and end-to-end connectivity.

**Project Folder:** `03-VLSM-Static-Routing`

### 04. Layer 3 Switching & SVI Inter-VLAN Routing

**Technologies:** Cisco 3560, Cisco 2960, SVIs, VLANs, 802.1Q, Layer 3 Switching

Built a simulated enterprise network with three departmental VLANs using a Cisco 3560 multilayer switch and Cisco 2960 access switches.

**Key Implementations:**
- Created Administration, HR, and IT VLANs.
- Configured trunk links between switches.
- Implemented Switch Virtual Interfaces (SVIs) as default gateways.
- Enabled IP routing on the multilayer switch.
- Verified directly connected routes and inter-VLAN connectivity.

**Project Folder:** `04-SVI-InterVLAN-Routing`

### 05. Extended ACLs & Network Segmentation

**Technologies:** Cisco IOS, Extended ACLs, SVIs, IPv4 Filtering

Extended the SVI routing lab by configuring a named extended Access Control List to restrict communication between departmental VLANs.

**Key Implementations:**
- Created an extended ACL to deny traffic from Administration to HR.
- Configured permit statements for other network traffic.
- Applied traffic filtering to a VLAN interface.
- Tested allowed and denied network communication.
- Investigated ACL placement, interface direction, and connectivity issues.

**Project Folder:** `05-Extended-ACL-Network-Security`

---

## Network Verification & Troubleshooting

Throughout these labs, I used Cisco IOS commands to inspect network configurations, verify connectivity, and troubleshoot routing and switching issues.

Common commands include:

```text
show ip interface brief
show ip route
show vlan brief
show interfaces trunk
show ip ospf neighbor
show ip protocols
show ip access-lists
show running-config
ping
traceroute
```

---

## Tools & Technologies

- Cisco Packet Tracer
- Cisco IOS CLI
- Cisco Routers
- Cisco Catalyst Layer 2 Switches
- Cisco Multilayer Switches
- IPv4 Networking
- OSPF
- VLANs and 802.1Q
- Static Routing
- VLSM
- Extended ACLs

---

## Certifications & Education

- CompTIA Security+ — Certified
- CompTIA Network+ — Certified
- Cisco CCNA — In Progress
- Bachelor of Science in Computer Networks and Cybersecurity

---

## Professional Development

I continue to expand my networking knowledge through hands-on labs, Cisco IOS configuration, troubleshooting scenarios, and CCNA studies.

My goal is to apply my enterprise IT support background and technical networking skills to network engineering and infrastructure-focused roles.

---

## Repository Information

Each project folder contains, or will contain:

- Cisco Packet Tracer (`.pkt`) lab files
- Network topology screenshots
- Configuration details
- Verification and testing results
- A dedicated README explaining the project

**Note:** All projects are simulated lab environments created for learning and technical skill development.
