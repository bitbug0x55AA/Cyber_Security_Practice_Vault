# Cyber Security Training Vault

> A comprehensive repository of practical labs, adversary emulation exercises, and defense engineering write-ups.

## 🎯 Overview

This repository serves as my primary staging ground and training vault. It chronicles my hands-on journey toward becoming a Purple Team expert, bridging the gap between offensive security tactics and proactive defense engineering. 

Rather than categorizing by training providers or certifications, the knowledge here is structured by **Technical Domains** to mirror industrial Security Operations Center (SOC) and Digital Forensics and Incident Response (DFIR) workflows.

*Note: For highly distilled tactical checklists, detection rules (Sigma/Yara), and IR playbooks derived from these exercises, please refer to my central playbook repository: `blue_team_hunting_field_notes`.*

## 📂 Repository Structure

```
    .
    ├── 00_Lab_Infrastructure/             
    │   ├── XCP-ng_Base_Setup/             
    │   ├── Active_Directory_Ranges/        
    │   └── Docker_and_Tooling/            
    │
    ├── 01_SOC_and_DFIR/                   
    │   ├── Log_Analysis_and_SIEM/          
    │   ├── Memory_and_Disk_Forensics/     
    │   ├── Network_Traffic_Analysis/      
    │   ├── Detection_Rule_Engineering/    
    │   └── End_to_End_Incidents/          
    │
    ├── 02_Malware_Analysis_and_Research/   
    │   ├── Basic_Static_and_Dynamic_Analysis/   
    │   └── Advanced_Malware_Research/     
    │
    ├── 03_Cyber_Threat_Intelligence/       
    │   ├── OSINT_and_Campaign_Tracking/   
    │   └── Threat_Modeling_Practices/     
    │
    └── 04_Offensive_Security/
        ├── 04.1_Recon_and_Enumeration/           
        ├── 04.2_Exploitation_Techniques/         
        ├── 04.3_Web_Application_Penetration/     
        ├── 04.4_Active_Directory_Attacks/        
        ├── 04.5_Post_Exploitation_and_Pivoting/  
        ├── 04.6_Integrated_Lab_Challenges/  
        └── 04.7_Full_Kill_Chain_Emulation/       
```

## 🏗️ Lab Infrastructure

All exercises and malware detonations are conducted within a strictly isolated, purpose-built bare-metal home lab environment running on **XCP-ng**. Network segregation, snapshots, and traffic routing are detailed within the `00_Lab_Infrastructure` directory to ensure reproducible testing.

---

*Maintained by Juana | Cyber Security Analyst* *Last Updated: March 2026*