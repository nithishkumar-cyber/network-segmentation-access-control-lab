# 🌐 Network Segmentation & Access Control Validation Lab (Packet Tracer)

🗓️ Date: April 2025  
📍 Tool: Cisco Packet Tracer  
🎯 Focus: Network segmentation design, access control enforcement, and traffic path validation in a simulated multi-router environment.

---

🎥 Video Walkthrough  
[▶️ Watch on Google Drive](https://drive.google.com/file/d/1pCSEznhMZSmdej0K9S7oCAp7shkYwAks/view)

📦 Also available in this repository:  
Download: `segmentation-lab.mkv`

---

# 🧠 Lab Overview

This lab demonstrates the design and validation of a segmented network using multiple routers, structured subnetting, static routing, DHCP configuration, and extended access control lists.

The objective was to validate how traffic flows across segmented networks and confirm that access control policies correctly restrict or allow communication between specific network segments.

The environment was built as a controlled simulation using Cisco Packet Tracer.

---

# 🏗️ Network Architecture

The network consists of three routers connected through separate subnets.

Key components include:

• Multiple segmented networks using structured subnetting  
• Static routing between routers  
• DHCP services providing automatic IP assignment  
• Extended Access Control Lists applied to router interfaces

Each subnet represents an isolated network segment with defined routing and access control behavior.

---

# 🔧 Key Configurations

### Static Routing

Manually configured route entries between routers to ensure packets follow intended paths.

Validated routing tables using:


show ip route


---

### DHCP Configuration

DHCP pools were configured on routers to automatically assign IP addresses to client systems.

Configuration included:

• IP address range  
• Default gateway assignment  
• Network mask definition

Client systems successfully received IP configuration dynamically.

---

### Access Control Enforcement

Extended ACL rules were implemented to control ICMP communication between selected subnets.

ACLs were applied to router interfaces to enforce segmentation policies.

Verification included:


show access-lists


This confirmed that restricted traffic was properly blocked while permitted traffic was allowed.

---

# 🔎 Validation & Testing

Traffic validation was performed using:

• `ping`  
• `traceroute`  
• router CLI inspection

Testing scenarios included verifying both permitted and restricted traffic paths between network segments.

---

# ✅ Test Results

| Test | Result | Observation |
|-----|-----|-----|
| PC1 ➜ PC2 ping | ✅ Allowed | Routing between segments operational |
| PC2 ➜ PC3 ping | ❌ Blocked | ACL policy enforced |
| PC1 ➜ PC3 ping | ✅ Allowed | Segmentation policy correctly configured |
| `show access-lists` | ✅ Hits logged | ACL filtering confirmed |
| `show ip route` | ✅ Valid | Static routes functioning |

---

# 📁 Repository Contents

`segmentation-lab.pkt` — Packet Tracer topology file  
`segmentation-lab.mkv` — Silent walkthrough of the lab environment  
`proof-of-function.txt` — Traffic validation observations

---

# 🧰 Skills Demonstrated

• Network segmentation fundamentals  
• Structured subnetting and IP planning  
• Static routing configuration  
• DHCP deployment and validation  
• Access control policy enforcement  
• Traffic path verification using CLI tools

---

# 🎯 Key Takeaway

This lab demonstrates how network segmentation and access control policies can be implemented and validated in a routed environment to enforce communication boundaries between network segments.

---

# ⚠️ Disclaimer

This project was conducted in a simulated lab environment using Cisco Packet Tracer for educational purposes.