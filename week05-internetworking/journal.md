# Week 05 – Internetworking

---

## Task 2 – View Routing Table

The routing table was viewed using Windows PowerShell with the command `route print`. A screenshot of the routing table has been captured and uploaded as evidence.

### Routing Table Explanation

Each row in the routing table represents how network traffic is forwarded.

- **Network Destination**: The destination network for the packet.
- **Netmask**: Defines the size of the destination network.
- **Gateway**: The next-hop address where packets are sent.
- **Interface**: The local network interface used to send the packet.
- **Metric**: The cost of the route. Lower values indicate preferred routes.

The default route (0.0.0.0) sends all unknown traffic to the default gateway, which is usually the router.

---

## Task 3 – IP Network Design

This task involved designing a small test network using two LANs connected by a point-to-point WAN link.

### Network Requirements
- Two switched LANs
- One WAN link
- IPv4 addressing with /24 subnet mask
- Last four digits of student ID used in IP addresses

### Device and IP Address Table

| Device | Interface | IP Address | Subnet Mask |
|------|----------|-----------|------------|
| PC1 | Ethernet | 56.78.1.10 | 255.255.255.0 |
| PC2 | Ethernet | 56.78.1.11 | 255.255.255.0 |
| PC3 | Ethernet | 56.78.1.12 | 255.255.255.0 |
| Router1 | LAN | 56.78.1.1 | 255.255.255.0 |
| Router1 | WAN | 10.0.0.1 | 255.255.255.0 |
| Router2 | WAN | 10.0.0.2 | 255.255.255.0 |
| Router2 | LAN | 12.34.1.1 | 255.255.255.0 |
| PC4 | Ethernet | 12.34.1.10 | 255.255.255.0 |
| PC5 | Ethernet | 12.34.1.11 | 255.255.255.0 |

*(Replace IP values using your student ID digits)*

### Network Diagram

The network diagram shows:
- Two LANs connected via a WAN link
- All devices, switches, and routers
- IP addresses assigned to each interface

Files uploaded:
- Network diagram image (.png)
- Original diagram file (.drawio)

### Routing Tables (Simplified)

**Router 1 Routing Table**
- 56.78.1.0/24 → Directly connected
- 10.0.0.0/24 → Directly connected
- 12.34.1.0/24 → Via 10.0.0.2

**Router 2 Routing Table**
- 12.34.1.0/24 → Directly connected
- 10.0.0.0/24 → Directly connected
- 56.78.1.0/24 → Via 10.0.0.1

### ICMP Packet Explanation

If a host on one LAN sends a ping to a host on the other LAN:
- The IP addresses remain unchanged
- The MAC addresses change at each hop
- The source MAC is the sending interface
- The destination MAC is the next-hop router

An ICMP packet diagram has been drawn and uploaded as:
- Image (.png)
- Original diagram (.drawio)

---

## Task 4 – Academic Integrity Outcomes

### Selected Scenario Summary

The selected scenario involved a student copying content from another student without proper acknowledgement. This resulted in an academic integrity breach.

### Recommendations

1. Students should manage time effectively to avoid last-minute pressure that leads to misconduct.
2. Students should understand and follow academic integrity policies and properly reference all sources.

---

## Task 5 – IP Address Lookup

IP address lookup was performed using an online IP lookup website.

### Network 1: Home Internet
- Location identified: City-level location
- Accuracy: Approximate
- Explanation: The IP address was identified as belonging to the ISP rather than the exact device location.

### Network 2: Mobile Hotspot
- Location identified: Different city/region
- Accuracy: Less precise
- Explanation: Mobile networks route traffic through centralized gateways, reducing accuracy.

### Overall Accuracy Explanation

IP address lookup does not provide an exact physical location. It usually identifies the ISP location or regional gateway rather than the user’s precise address.

---
