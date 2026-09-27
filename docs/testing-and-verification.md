# Testing & Verification

## Switch

Check VLANs:

```text
show vlan brief
```

Check trunk:

```text
show interfaces trunk
```

## Router

Check interfaces:

```text
show ip interface brief
```

Check DHCP bindings:

```text
show ip dhcp binding
```

Check routes:

```text
show ip route
```

## Connectivity

From a PC, test the gateways:

```text
ping 192.168.10.1
ping 192.168.20.1
ping 192.168.30.1
```

Test inter-VLAN communication after confirming gateway connectivity.
