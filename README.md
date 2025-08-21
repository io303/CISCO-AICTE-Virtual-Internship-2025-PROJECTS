# CISCO-AICTE-Virtual-Internship-2025-PROJECTS
Networking Industry Problem Statement - Cisco VIP 2025


📌 Overview

This project is developed as part of the Cisco Virtual Internship Program 2025 (Networking Stream).
The goal is to design and implement a tool that can automatically generate network topologies from router configuration files, validate configurations, simulate network activities, and recommend optimizations.

🎯 Problem Statement

Currently, there is no automated solution to generate a hierarchical network topology directly from router configuration files.
This project aims to:

Parse router/switch configuration files.

Build a hierarchical network topology.

Validate configurations (e.g., duplicate IPs, incorrect VLAN labels, wrong gateways).

Analyze bandwidth capacity & recommend load balancing.

Simulate Day-1 & Day-2 network activities, including link failures and fault injection.

🛠 Features

Network Topology Generation

Automatic creation of hierarchical topology.

Awareness of link bandwidth and traffic load.

Network Performance & Load Management

Load balancing suggestions for high-traffic scenarios.

Application-aware traffic management.

Configuration Validation & Optimization

Detect missing configs (e.g., switch files).

Identify duplicate IPs, MTU mismatches, VLAN issues, loops.

Recommend node aggregation & protocol choices (BGP vs OSPF).

Simulation & Fault Injection

Day-1 simulation (ARP, neighbor discovery, OSPF discovery).

Link failure impact analysis.

Pause & resume simulations for testing.

Implementation Architecture

Multithreading for routers/switches.

Inter-process communication (FIFO / TCP/IP).

Statistics & logs at thread/node levels.

Optional real IP packet creation.

📂 Project Workflow

Input: Directory containing configuration files, e.g.

Conf/R1/config.dump  
Conf/R2/config.dump  
Conf/R3/config.dump  


Tool parses configs → generates network topology.

Validate network setup & recommend optimizations.

Run simulations & analyze failure scenarios.

🚀 Tech Stack

Programming Language: (Python / C++ / Java – specify your choice)

Networking Concepts: VLANs, OSPF, BGP, ARP, MTU, Load Balancing.

Concurrency: Multithreading for simulating devices.

IPC: FIFO / TCP-IP for metadata exchange.

📑 Future Enhancements

GUI-based topology visualization.

Real packet-level simulation.

AI/ML-based traffic optimization.

👨‍💻 Contributors

Rahul Singh – Cisco Networking Academy Intern

Guided by G L Bajaj Institute of Technology and Management

🏅 Acknowledgement

Special thanks to Cisco Networking Academy and Mohit Sharma (Instructor) for guidance and mentorship throughout this project.
