# Build Guide — Cisco Packet Tracer

## 1. Add Devices

Create:
- 1 Cisco router with a GigabitEthernet interface
- 1 Cisco switch
- 3 PCs

Name them R1, SW1, PC1, PC2 and PC3.

## 2. Connect Devices

- R1 G0/0 → SW1 G0/1
- PC1 → SW1 F0/1
- PC2 → SW1 F0/2
- PC3 → SW1 F0/3

## 3. Configure SW1

Use `configs/SW1-switch-config.txt`.

## 4. Configure R1

Use `configs/R1-router-config.txt`.

## 5. Configure PCs

Set each PC to obtain an IP address automatically using DHCP.

## 6. Verify

Expected address ranges:
- PC1 → 192.168.10.x
- PC2 → 192.168.20.x
- PC3 → 192.168.30.x

## 7. Test Connectivity

Test each PC's default gateway and then inter-VLAN communication.

## 8. Save Your Packet Tracer File

After successful testing, save it as `cisco-vlan-networking-lab.pkt` and add it to the repository root.
