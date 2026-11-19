
# Inter-VLAN Routing Using SVIs | Cisco Packet Tracer

## Project Overview
This lab demonstrates inter-VLAN routing using
Switch Virtual Interfaces (SVIs) on a Cisco 3560
multilayer switch.

The network consists of three departments:
Administration, Human Resources, and IT.

## Network Topology
![Network Topology](screenshots/topology.png)

## Technologies Used
- Cisco Packet Tracer
- Cisco IOS
- Cisco 3560 Layer 3 Switch
- Cisco 2960 Access Switches
- VLANs and 802.1Q Trunking
- Switch Virtual Interfaces (SVIs)
- IPv4 Addressing and Inter-VLAN Routing

## IP Addressing Scheme

| VLAN | Department | Subnet | Gateway |
|---|---|---|---|
| 10 | Administration | 192.168.10.0/24 | 192.168.10.1 |
| 20 | Human Resources | 192.168.20.0/24 | 192.168.20.1 |
| 30 | IT | 192.168.30.0/24 | 192.168.30.1 |

## Configuration Highlights
1. Created VLANs 10, 20, and 30.
2. Configured access and trunk ports.
3. Created SVIs as VLAN default gateways.
4. Enabled IP routing on the multilayer switch.
5. Configured static IP addresses.

## Verification and Testing
Validated VLAN configuration, trunk status,
SVI operation, and routing using:

```text
show vlan brief
show interfaces trunk
show ip interface brief
show ip route
ping 192.168.20.10
ping 192.168.30.10
```

### Routing Table
![Routing Table](screenshots/routing-table.png)

### Connectivity Test
![Ping Test](screenshots/ping-test.png)

## Key Takeaways
This lab reinforced how SVIs provide Layer 3
gateways for VLANs and how a multilayer switch
enables routing between separate IP subnets.

## Lab File
[Download Packet Tracer Lab](Inter-VLAN-Routing-Using-SVIs.pkt)
  
