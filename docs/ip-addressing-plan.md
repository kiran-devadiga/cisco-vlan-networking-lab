# IP Addressing Plan

| VLAN ID | Name | Network | Gateway |
|---|---|---|---|
| 10 | MANAGEMENT | 192.168.10.0/24 | 192.168.10.1 |
| 20 | SUPPORT | 192.168.20.0/24 | 192.168.20.1 |
| 30 | ADMIN | 192.168.30.0/24 | 192.168.30.1 |

The router provides DHCP for all three VLANs.

Reserved gateway ranges:

- VLAN 10: 192.168.10.1–192.168.10.10
- VLAN 20: 192.168.20.1–192.168.20.10
- VLAN 30: 192.168.30.1–192.168.30.10
