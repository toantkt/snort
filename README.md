# Snort Network Intrusion Prevention System

![IPS](https://img.shields.io/badge/IPS-Snort-red)
![Detection](https://img.shields.io/badge/Detection-Custom%20Rules-orange)
![Network](https://img.shields.io/badge/Network-Security-green)

## Overview

This project demonstrates the deployment and configuration of Snort as an inline Intrusion Prevention System (IPS) to detect and block malicious network traffic.

The project focuses on developing custom detection signatures, validating rule effectiveness against real attack traffic, and evaluating signature-based prevention techniques within a controlled virtual environment.

## Objectives

- Deploy Snort in inline IPS mode
- Configure signature-based intrusion prevention
- Develop custom Snort detection rules
- Detect and block common network attacks
- Validate IPS effectiveness through attack simulation
- Analyze network traffic before and after rule deployment

## Repository Structure

```text
snort/
│
├── img/
│   └── topology.png 
│
├── LICENSE
│
├── README.md
│
└── Report.pdf
```

## Network Topology

![Topology](img/topology.png)

## Technology Stack

- Snort IDS/IPS
- Metasploit Framework
- Nmap
- Wireshark
- VMware Workstation
- Kali Linux
- Ubuntu Server

## Implementation

### IPS Deployment

Configured Snort in inline Intrusion Prevention System (IPS) mode to inspect and actively block malicious traffic traversing the network.

Deployment included:

- Inline packet inspection
- Rule loading
- Traffic monitoring
- Alert generation
- Packet blocking

### Custom Rule Development

Developed custom Snort signatures to identify and prevent known attack patterns.

Rules were created for:

- Nmap OS Fingerprinting
- PHP CGI Argument Injection
- UnrealIRCd Backdoor Exploitation

Each rule was validated using live attack traffic generated from the attacker machine.

### Attack Simulation

Performed controlled offensive security testing to evaluate IPS detection and prevention capabilities.

Attack techniques included:

- Network reconnaissance
- Operating system fingerprinting
- Remote exploitation
- Payload delivery

### Traffic Analysis

Captured and analyzed network traffic to compare system behavior before and after IPS enforcement.

Analysis included:

- Packet inspection
- Signature matching
- Alert validation
- Blocked connection verification

## Validation & Testing

| Attack | Detection | Prevention |
| --------- | ----------- | ------------ |
| Nmap OS Fingerprinting | ✅ | ✅ |
| PHP CGI Argument Injection | ✅ | ✅ |
| UnrealIRCd Backdoor Exploitation | ✅ | ✅ |

## Key Findings

- Snort successfully detects and blocks known attack signatures when deployed in inline IPS mode.
- Well-designed custom rules significantly improve protection against targeted attack techniques.
- Signature tuning is essential to minimize false positives while maintaining detection accuracy.
- Packet-level analysis provides valuable insight into rule behavior and attack characteristics.

## Skills Developed

### Network Security

- Intrusion Prevention Systems (IPS)
- Signature-Based Detection
- Network Traffic Inspection
- Packet Analysis

### Detection Engineering

- Snort Rule Development
- Signature Tuning
- Rule Validation
- False Positive Analysis

### Offensive Security

- Nmap Reconnaissance
- Exploit Validation
- Attack Simulation
- Penetration Testing

### Security Testing

- IPS Evaluation
- Detection Validation
- Security Control Testing
- Attack Replay

### Digital Forensics

- Packet Capture Analysis
- Alert Investigation
- Network Evidence Collection
- Traffic Verification
