# Cyber Security Training Vault

> A comprehensive repository of practical labs, adversary emulation exercises, and defense engineering write-ups.

## 🎯 Overview

This repository serves as my primary staging ground and training vault. It chronicles my hands-on journey toward becoming a Purple Team expert, bridging the gap between offensive security tactics and proactive defense engineering. 

Rather than categorizing by training providers or certifications, the knowledge here is structured by **Technical Domains** to mirror industrial Security Operations Center (SOC) and Digital Forensics and Incident Response (DFIR) workflows.

*Note: For highly distilled tactical checklists, detection rules (Sigma/Yara), and IR playbooks derived from these exercises, please refer to my central playbook repository: `blue_team_hunting_field_notes`.*

## 📂 Repository Structure

```
    .
    ├── 00_Lab_Infrastructure/              # Home lab architecture and automation
    │   ├── XCP-ng_Base_Setup/              # Foundational hypervisor configurations & Inventory
    │   ├── Active_Directory_Ranges/        # AD ranges for exploitation & detection testing
    │   └── Docker_and_Tooling/             # Containerized pipelines
    │
    ├── 01_SOC_and_DFIR/                    # Defensive operations and response
    │   ├── Log_Analysis_and_SIEM/          # Splunk/ELK hunting hypotheses and queries
    │   ├── Memory_and_Disk_Forensics/      # Artifact extraction and memory analysis
    │   ├── Network_Traffic_Analysis/       # PCAP analysis and NIDS signature testing
    │   ├── Detection_Rule_Engineering/     # Testing and validating Sigma/Yara rules
    │   └── End_to_End_Incidents/           # Multi-domain defense labs
    │
    ├── 02_Malware_Analysis_and_Research/   # Reverse engineering and malware behavior
    │   ├── Static_and_Dynamic_Analysis/    # Triage and behavioral analysis notes
    │   └── Advanced_Malware_Research/      # Deep dives into specific malware families
    │
    ├── 03_Cyber_Threat_Intelligence/       # Threat profiling and OSINT
    │   ├── OSINT_and_Campaign_Tracking/    # Open-source intelligence practicals
    │   └── Threat_Modeling_Practices/      # Adversary infrastructure mapping
    │
    └── 04_Offensive_Security/              # Adversary emulation and exploitation
        ├── Penetration_Testing_Basics/     # Vulnerability assessment records
        ├── AD_Exploitation/                # Attack chain reproduction
        ├── Adversary_Emulation/            # Isolated red team exercises and AE plans
        └── Full_Kill_Chain_Emulation/      # End-to-end multi-stage targets
```

## 🏗️ Lab Infrastructure

All exercises and malware detonations are conducted within a strictly isolated, purpose-built bare-metal home lab environment running on **XCP-ng**. Network segregation, snapshots, and traffic routing are detailed within the `00_Lab_Infrastructure` directory to ensure reproducible testing.

## 📜 Write-up Standard

To maintain consistency across all technical domains, every new lab or case study documented in this repository follows a unified reporting structure:

1. **Executive Summary / Scenario**: A brief overview of the incident, malware, or target box.
2. **Environment & Tools**: Lab setup, IP ranges, and specific tools utilized (e.g., x64dbg, Volatility 3, Splunk).
3. **Analysis / Attack Chain**: The step-by-step technical methodology, including screenshots, command snippets, and raw logs.
4. **Indicators of Compromise (IOCs)**: Hashes, IPs, domains, or memory signatures identified.
5. **Detection & Mitigation**: How to spot this activity in a production environment (SIEM queries, EDR telemetry).

---

*Maintained by Juana | Cyber Security Analyst* *Last Updated: March 2026*