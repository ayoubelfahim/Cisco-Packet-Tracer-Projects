# VLAN Segmentation with Inter-VLAN Routing

## Overview

This project demonstrates VLAN segmentation and Inter-VLAN Routing using Cisco Packet Tracer.

Two departments are separated into different VLANs while maintaining communication through Router-on-a-Stick.

---

## Objectives

- Create VLANs
- Configure access ports
- Configure an IEEE 802.1Q trunk
- Configure Router-on-a-Stick
- Verify communication between VLANs

---

## Technologies

- Cisco Packet Tracer
- Cisco IOS CLI
- VLAN
- IEEE 802.1Q
- Router-on-a-Stick
- Inter-VLAN Routing
- ICMP

---

## Network Design

### VLAN 10

- Department: Administration
- Network: 192.168.10.0/24
- Gateway: 192.168.10.1

### VLAN 20

- Department: Development
- Network: 192.168.20.0/24
- Gateway: 192.168.20.1

---

## Switch Configuration

- Create VLAN 10
- Create VLAN 20
- Assign access ports
- Configure trunk port (802.1Q)

---

## Router Configuration

Router-on-a-Stick configuration:

- GigabitEthernet0/0.10
- GigabitEthernet0/0.20

Configured using:

- encapsulation dot1Q
- ip address
- no shutdown

---

## Verification

- Verify VLAN membership
- Verify trunk status
- Verify router subinterfaces
- Successful ping between VLAN 10 and VLAN 20

---

## Skills

- VLAN Configuration
- Inter-VLAN Routing
- Router-on-a-Stick
- Cisco IOS CLI
- Switch Configuration
- Network Segmentation
- Network Troubleshooting

---

## Files

- vlan-inter-vlan-routing.pkt
- network-topology.png
- switch-vlan-configuration.png
- router-inter-vlan-configuration.png
- connectivity-test.png

---

## Screenshots

### Network Topology

![Network Topology](network-topology.png)

---

### Switch VLAN Configuration

![Switch VLAN Configuration](switch-vlan-configuration.png)

---

### Router Configuration

![Router Configuration](router-inter-vlan-configuration.png)

---

### Connectivity Test

![Connectivity Test](connectivity-test.png)

---

## What I Learned

- Design VLAN-based networks
- Configure VLANs and access ports
- Configure IEEE 802.1Q trunk links
- Configure Router-on-a-Stick
- Implement Inter-VLAN Routing
- Verify connectivity using ICMP
