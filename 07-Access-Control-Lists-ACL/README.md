# Access Control Lists (ACL)

## Overview

This project demonstrates the configuration of **Standard** and **Extended Access Control Lists (ACL)** using Cisco Packet Tracer.

ACLs are used to control network traffic by permitting or denying packets based on source addresses, destination addresses, and protocols.

---

## Objectives

- Configure Standard ACLs
- Configure Extended ACLs
- Apply ACLs to router interfaces
- Verify ACL operation
- Test permitted and denied traffic

---

## Technologies

- Cisco Packet Tracer
- Cisco IOS CLI
- IPv4
- Standard ACL
- Extended ACL
- ICMP
- Network Security

---

# Network Topology

![Network Topology](network-topology.png)

---

# Standard ACL Configuration

![Standard ACL Configuration](acl-standard-config.png)

### Purpose

The Standard ACL filters traffic based on the **source IP address**.

---

# Standard ACL Verification

![Standard ACL Verification](show-access-lists-standard.png)

This output verifies that the Standard ACL has been configured successfully.

---

# Extended ACL Configuration

![Extended ACL Configuration](acl-extended-config.png)

### Purpose

The Extended ACL filters traffic based on:

- Source IP Address
- Destination IP Address
- Protocol
- ICMP

This provides more granular traffic control.

---

# Extended ACL Verification

![Extended ACL Verification](show-access-lists-extended.png)

The output confirms that the Extended ACL is correctly configured and active.

---

# Connectivity Test (Denied Traffic)

![Denied Ping Test](extended-acl-ping-test.png)

The ICMP traffic from **LAN1 (192.168.1.0/24)** to **LAN3 (192.168.3.0/24)** is successfully blocked by the Extended ACL.

---

# Connectivity Test (Allowed Traffic)

![Allowed Ping Test](extended-acl-allowed-ping.png)

Traffic that is not matched by the deny rule is successfully permitted, confirming the ACL policy works as expected.

---

## What I Learned

- Configure Standard ACLs
- Configure Extended ACLs
- Apply ACLs to router interfaces
- Verify ACLs using Cisco IOS commands
- Control network traffic using security policies
- Troubleshoot ACL configurations
- Test permitted and denied ICMP traffic

---

## Project Files

```text
07-Access-Control-Lists-ACL/
│── README.md
│── Project 07.pkt
│── network-topology.png
│── acl-standard-config.png
│── show-access-lists-standard.png
│── acl-extended-config.png
│── show-access-lists-extended.png
│── extended-acl-ping-test.png
│── extended-acl-allowed-ping.png
```

---

## Skills

- Cisco Packet Tracer
- Cisco IOS
- IPv4
- Standard ACL
- Extended ACL
- ICMP
- Network Security
- Access Control
- Cisco CLI
- Network Troubleshooting
