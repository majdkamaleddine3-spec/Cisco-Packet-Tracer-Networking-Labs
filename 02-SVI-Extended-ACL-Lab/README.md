# Extended ACL Network Security Lab | Cisco Packet Tracer

## Project Overview

Implemented an extended Access Control List (ACL) on a Cisco 3560 multilayer switch to enforce network segmentation policies between departmental VLANs.

This project builds upon a previously configured SVI inter-VLAN routing lab, introducing Layer 3 traffic filtering to control communication between Administration, Human Resources, and IT networks.

## Lab Objectives

- Configure a named extended ACL using Cisco IOS.
- Restrict traffic from Administration (VLAN 10) to Human Resources (VLAN 20).
- Permit communication between IT (VLAN 30) and other departments.
- Apply an ACL inbound on a Switch Virtual Interface (SVI).
- Verify ACL behavior using connectivity testing and Cisco IOS commands.

## Network Addressing

| Department | VLAN | Network |
|---|---|---|
| Administration | 10 | 192.168.10.0/24 |
| Human Resources | 20 | 192.168.20.0/24 |
| IT | 30 | 192.168.30.0/24 |

## Security Policy

| Source | Destination | Action |
|---|---|---|
| ADMIN | HR | Deny |
| ADMIN | IT | Permit |
| IT | HR | Permit |
| IT | ADMIN | Permit |

## Extended ACL Configuration

```text
ip access-list extended ADMIN-HR-BLOCK
 10 deny ip 192.168.10.0 0.0.0.255 192.168.20.0 0.0.0.255
 20 permit ip any any

interface vlan 10
 ip access-group ADMIN-HR-BLOCK in
```

The ACL is designed to block IP traffic originating from the Administration subnet and destined for the HR subnet, while allowing other traffic.

## Verification Commands

```text
show ip access-lists
show ip interface vlan 10
show running-config
```

## Connectivity Testing

| Test | Expected Result |
|---|---|
| ADMIN → HR | Blocked |
| ADMIN → IT | Successful |
| IT → HR | Successful |
| IT → ADMIN | Successful |

## Troubleshooting

Investigated ACL configuration and interface assignments to determine whether traffic restrictions were caused by ACL filtering or underlying connectivity issues.

Verified ACL placement, rule ordering, and interface direction.

## Key Takeaways

- Practiced configuring extended ACLs to enforce network access policies.
- Learned how ACL placement and direction affect traffic filtering.
- Reinforced understanding of source and destination wildcard masks.
- Developed troubleshooting skills by analyzing permitted and denied traffic between VLANs.

## Packet Tracer File

[Download Extended ACL Lab](Extended-ACL.pkt)
