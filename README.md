# Cyber Homelab (SOC/Blue Team Simulation)

## 📌 Overview
A cybersecurity homelab project with pfSense, Security Onion, Splunk, Active Directory, and attack/defense machines.  
Purpose: Learn SOC workflows, simulate attacks, and detect them using enterprise-grade tools.

## 🖥️ Lab Topology
![Network Diagram](diagrams/topology.png)

## ⚙️ Environment Setup
- Host: 16GB RAM, VMware Workstation
- VMs: pfSense, Security Onion, Splunk, Windows Server (DC), Windows 10, Kali Linux

## 📸 Screenshots
Screenshots are organized under `/exports/`

## Results

Successfully captured user logon events from the Domain Controller.

Verified failed logons (4625) and successful logons (4624) appeared in Splunk in real time.

This enables basic authentication monitoring, which is critical for detecting brute force attacks and unauthorized access.

## Next Steps

Correlate brute force activity (multiple 4625 events → single 4624).

Alert on suspicious logon patterns (e.g., logon outside business hours).
