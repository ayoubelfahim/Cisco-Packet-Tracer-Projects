 # Dynamic Routing with RIPv2

## Overview

This project demonstrates **Dynamic Routing using RIP Version 2 (RIPv2)** in Cisco Packet Tracer.

Three separate LANs are interconnected through multiple routers. Instead of using static routes, RIPv2 dynamically exchanges routing information, allowing all networks to communicate automatically.

---

## Objectives

- Configure Dynamic Routing using RIPv2
- Advertise IPv4 networks
- Disable automatic route summarization
- Verify routing tables
- Test end-to-end connectivity

---

## Network Topology

![Network Topology](network-topology.png)

---

## Network Scenario

The topology consists of three office networks connected through two WAN point-to-point links.

- **Branch Office**
  - LAN1: `192.168.1.0/24`

- **Core Network**
  - LAN2: `192.168.2.0/24`

- **Remote Office**
  - LAN3: `192.168.3.0/24`

Routers exchange routing information automatically using **RIP Version 2**, eliminating the need for manually configured static routes.

---

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS
- IPv4
- Dynamic Routing
- RIP Version 2 (RIPv2)
- ICMP

---

## IP Addressing Plan

| Network | Address |
|---------|---------|
| LAN 1 | 192.168.1.0/24 |
| LAN 2 | 192.168.2.0/24 |
| LAN 3 | 192.168.3.0/24 |
| WAN Link 1 | 10.0.0.0/30 |
| WAN Link 2 | 10.0.0.4/30 |

---

## Router Configuration

### R1 (Branch)

- Configure RIP Version 2
- Advertise:
  - LAN1
  - LAN2
  - WAN Link 1

### R2 (Core)

- Configure RIP Version 2
- Advertise:
  - WAN Link 1
  - WAN Link 2

### R3 (Remote)

- Configure RIP Version 2
- Advertise:
  - LAN3
  - WAN Link 2

---

## RIP Configuration

### R1

![R1 RIP Configuration](rip-configuration-r1.png)

### R2

![R2 RIP Configuration](rip-configuration-r2.png)

### R3

![R3 RIP Configuration](rip-configuration-r3.png)

---

## Routing Tables

### Routing Table (R1)

![Routing Table R1](routing-table-r1.png)

### Routing Table (R2)

![Routing Table R2](routing-table-r2.png)

### Routing Table (R3)

![Routing Table R3](routing-table-r3.png)

---

## Connectivity Test

### Branch to Remote

![Branch to Remote](branch-to-remote-ping.png)

### Remote to Branch

![Remote to Branch](remote-to-branch-ping.png)

---

## Verification Commands

The following Cisco IOS commands were used during verification:

```bash
show ip interface brief
show ip protocols
show ip route
ping
```

---

## Skills Demonstrated

- Dynamic Routing
- RIP Version 2 (RIPv2)
- Cisco IOS CLI
- IPv4 Addressing
- Routing Tables
- WAN Configuration
- ICMP Connectivity Testing
- Network Troubleshooting

---

## Project Files

```
rip-routing.pkt
network-topology.png
rip-configuration-r1.png
rip-configuration-r2.png
rip-configuration-r3.png
routing-table-r1.png
routing-table-r2.png
routing-table-r3.png
branch-to-remote-ping.png
remote-to-branch-ping.png
README.md
LICENSE
```

---

## Conclusion

This project demonstrates how **RIP Version 2** enables routers to automatically exchange routing information, allowing seamless communication between multiple LANs without manually configuring static routes. The routing tables were successfully learned through RIP, and end-to-end connectivity was verified using ICMP ping tests.
