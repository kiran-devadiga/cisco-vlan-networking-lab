# Cisco VLAN & Inter-VLAN Routing Lab

A Cisco Packet Tracer networking lab demonstrating VLAN segmentation, 802.1Q trunking, Router-on-a-Stick inter-VLAN routing, DHCP, and basic troubleshooting.

## Project Overview

This project simulates a small organization's network with three departments:

- Management — VLAN 10
- Support — VLAN 20
- Admin — VLAN 30

A Cisco router provides inter-VLAN routing and DHCP services, while a Cisco switch provides VLAN segmentation.

## Network Topology

```text
                    R1
              Router-on-a-Stick
                     |
                 802.1Q Trunk
                     |
                    SW1
              _______|_______
             /       |       \\
          PC1       PC2       PC3
        VLAN 10    VLAN 20   VLAN 30
     Management   Support     Admin
```

## IP Addressing Plan

| VLAN | Department | Network | Default Gateway |
|---|---|---|---|
| 10 | Management | 192.168.10.0/24 | 192.168.10.1 |
| 20 | Support | 192.168.20.0/24 | 192.168.20.1 |
| 30 | Admin | 192.168.30.0/24 | 192.168.30.1 |

## Technologies Used

- Cisco Packet Tracer
- IPv4
- VLAN
- 802.1Q Trunking
- Router-on-a-Stick
- Inter-VLAN Routing
- DHCP
- Cisco IOS CLI
- Basic Network Troubleshooting

## Files

- `configs/R1-router-config.txt` — Router configuration reference
- `configs/SW1-switch-config.txt` — Switch configuration reference
- `docs/ip-addressing-plan.md` — Addressing plan
- `docs/testing-and-verification.md` — Verification commands
- `docs/troubleshooting.md` — Common troubleshooting scenarios
- `docs/build-guide.md` — Steps to recreate the lab in Packet Tracer
- `topology/topology.txt` — Text topology diagram

> The configuration files are reference configurations. Create and test the Packet Tracer `.pkt` file locally before adding it to this repository.

## Learning Outcomes

- Creating and assigning VLANs
- Configuring access and trunk ports
- Configuring router subinterfaces
- Implementing inter-VLAN routing
- Configuring DHCP
- Verifying network status
- Troubleshooting basic connectivity issues

## Author

**Kiran Krishna Devadiga**  
Technical Support Engineer | Networking & Cloud Enthusiast
