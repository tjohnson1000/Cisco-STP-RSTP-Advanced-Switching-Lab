# Cisco STP & RSTP Advanced Switching Lab
<img src="https://i.imgur.com/HNzguPb.png" height="80%" alt="[name of screenshot]" />
## Overview
This CCNA/CCNP-level lab explores **Spanning Tree Protocol (STP)** and **Rapid Spanning Tree Protocol (RSTP)** in a multi-switch environment. It provides hands-on experience with **PVST+**, **Rapid PVST**, **Root Bridge elections**, and advanced loop prevention mechanisms like **PortFast, Root Guard, BPDU Guard, BPDU Filter, and Loop Guard**.

## Lab Topology
- **Switches**: DS-1, DS-2, AS-1, AS-2
- **VLANs**: VLAN 10, VLAN 20
- **PCs** connected for end-host simulation

## Objectives
1. Configure basic switch settings and VLAN interfaces
2. Verify STP operation and convergence
3. Implement and test Rapid PVST
4. Control Root Bridge elections using priorities
5. Use PortFast to speed up host connectivity
6. Prevent topology manipulation using Root Guard
7. Protect edge ports with BPDU Guard
8. Suppress BPDUs using BPDU Filter
9. Prevent loops with Loop Guard

## Key Features Covered
- **STP Role Verification**: Identify Root, Designated, and Alternate ports
- **MAC-based Root Bridge Election**
- **Priority Manipulation**: `spanning-tree vlan [vlan-id] root [primary|secondary]`
- **Port Cost & Priority Tuning** for root path selection
- **Transition to Rapid PVST** for faster convergence
- **Event Debugging**: `debug spanning-tree events`
- **BPDU-Based Protections**: BPDU Guard, Filter, Loop Guard

## Verification Commands
```bash
show spanning-tree
show spanning-tree vlan [id]
show spanning-tree root
show spanning-tree interface [int] detail
show spanning-tree inconsistentports
debug spanning-tree events
```

## Repository Structure
```
├── configs/
│   ├── DS-1_Config.txt
│   ├── DS-2_Config.txt
│   ├── AS-1_Config.txt
│   ├── AS-2_Config.txt
├── README.md
├── screenshots/
└── topology.png
```

## Conclusion
This lab demonstrates a deep understanding of **STP and RSTP behavior**, including convergence, elections, and advanced protection mechanisms. It’s ideal for engineers preparing for **CCNA/CCNP switching exams** or designing robust Layer 2 enterprise networks.

---
**Author:** Travis Johnson  
**Company:** 10Digit Solutions LLC  
**GitHub Repository:** [Add link when available]
