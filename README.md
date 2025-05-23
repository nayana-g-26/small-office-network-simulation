# 🏢 Small Office Network Simulation (Cisco Packet Tracer)

This project simulates a small office LAN setup using **Cisco Packet Tracer**, demonstrating basic networking concepts including IP addressing, static routing, and server access.

## 🎯 Objective

To build and simulate a functional small office network that allows:
- Communication between multiple subnets
- Access to a central server
- Understanding of routing and switching concepts

---

## 🖥️ Topology Overview

The network includes:
- 2 Routers
- 4 Switches
- 6 PCs
- 1 Server

Each subnet is connected via a router, and IPs are statically assigned. The server provides centralized services to all client devices.

### 📷 Network Diagram

![network_topology](https://github.com/user-attachments/assets/1d2aea49-395a-4acd-bed0-9d697d0fb251)

---

## 📄 IP Addressing Plan

All IPs are organized by subnet. Refer to this for details:

| **Device**    | **Interface** | **IP Address** | **Subnet**     | **Notes**                 |
| ------------- | ------------- | -------------- | -------------- | ------------------------- |
| **Router R1** | G0/0          | 192.168.1.254  | 192.168.1.0/24 | Connected to Server + SW1 |
|               | G0/1          | 192.168.2.254  | 192.168.2.0/24 | Connected to SW2          |
|               | G1/0          | 192.168.3.254  | 192.168.3.0/24 | Connected to SW3          |
|               | G1/1          | 192.168.4.254  | 192.168.4.0/24 | Connected to SW4          |
| **Server**    | —             | 192.168.1.100  | 192.168.1.0/24 | Connected to SW1          |
| **PC0**       | —             | 192.168.2.1    | 192.168.2.0/24 | Connected to SW2          |
| **PC1**       | —             | 192.168.2.2    | 192.168.2.0/24 | Connected to SW2          |
| **PC2**       | —             | 192.168.3.1    | 192.168.3.0/24 | Connected to SW3          |
| **PC3**       | —             | 192.168.3.2    | 192.168.3.0/24 | Connected to SW3          |
| **PC4**       | —             | 192.168.4.1    | 192.168.4.0/24 | Connected to SW4          |
| **PC5**       | —             | 192.168.4.2    | 192.168.4.0/24 | Connected to SW4          |

---

## 🚀 How to Run the Simulation

1. Install [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer).
2. Download this repository.
3. Open the `.pkt` file in Cisco Packet Tracer.
4. Use the simulation panel to test ping commands and inspect routing.

---

## ✅ Features

- Static routing configuration
- Centralized server access
- LAN segmentation with subnetting

---

## 🌟 Future Improvements

- Add DHCP server and dynamic IP allocation
- Implement VLANs and inter-VLAN routing
- Add firewall and security policies
