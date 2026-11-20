# VLSM Subnetting & Static Routing | Cisco Packet Tracer

## Project Overview

Designed and configured a simulated enterprise network consisting of three routers, three LANs, and two point-to-point WAN links. Implemented Variable Length Subnet Masking (VLSM) to efficiently allocate IP addresses and configured static routing to establish connectivity between geographically separated networks.

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS
- IPv4 Addressing
- VLSM Subnetting
- Static Routing
- Default Routes
- Routing Table Analysis
- ICMP and Traceroute

## Network Design

| Network | Subnet | Purpose |
|---|---|---|
| HQ LAN | 192.168.5.0/26 | 50 hosts |
| Branch 1 LAN | 192.168.5.64/27 | 25 hosts |
| Branch 2 LAN | 192.168.5.96/28 | 12 hosts |
| HQ–Branch 1 WAN | 192.168.5.112/30 | Point-to-point |
| HQ–Branch 2 WAN | 192.168.5.116/30 | Point-to-point |

## Configuration Summary

- Calculated VLSM subnet allocations based on host requirements.
- Configured router interfaces with appropriate IPv4 addresses and subnet masks.
- Implemented static routes and default routes for inter-network communication.
- Verified routing tables and connectivity using Cisco IOS commands.
- Tested end-to-end connectivity between all three LANs.

## Verification Commands

```text
show ip interface brief
show ip route
show running-config
ping
traceroute
```

## Key Takeaways

This lab strengthened my understanding of IP subnet planning, routing decisions, next-hop addresses, and static route configuration. It also reinforced troubleshooting techniques for diagnosing connectivity issues across multiple routed networks.

## Packet Tracer File

[Download VLSM & Static Routing Lab](VLSM-Static-Routing.pkt)
