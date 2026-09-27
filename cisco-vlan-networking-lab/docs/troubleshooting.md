# Troubleshooting Guide

## PC receives no IP address

Check:
1. PC is set to DHCP.
2. Correct switch access VLAN is assigned.
3. Trunk is operational.
4. Router subinterface exists for the VLAN.
5. DHCP pool uses the correct network.

Useful commands:

```text
show vlan brief
show interfaces trunk
show ip dhcp binding
```

## Inter-VLAN ping fails

Check:
1. Router physical interface is enabled.
2. Router subinterface has the correct VLAN ID.
3. `encapsulation dot1Q` matches the VLAN.
4. PC default gateway is correct.
5. Switch-to-router link is a trunk.

## VLAN is not working

Run:

```text
show vlan brief
```

Verify the access port is assigned to the expected VLAN.

## Trunk is not working

Run:

```text
show interfaces trunk
```

Confirm VLANs 10, 20 and 30 are permitted on the trunk.
