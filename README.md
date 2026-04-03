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

## 🗺️ Learning Roadmap (2025 - 2028)

<details>
<summary><b>Click to expand my path to Purple Team Expert</b></summary>

This roadmap tracks my continuous progression toward becoming a Purple Team expert. It balances offensive mastery with defensive engineering.

### ✅ Completed Milestones
* **2026 Q1**: **BTL1** (Blue Team Level 1) - *Certified*
* **2026 Q1**: **MAD20** Adversary Emulation Methodology - *Completed*
* **2025 Q4**: **MAD20** Cyber Threat Intelligence & SOC Assessment - *Completed*
* **2025 Q4**: **eJPT** (Junior Penetration Tester) Path - *Completed*

### 🚀 Currently Processing
* **HTB CDSA** (Certified Detection Systems Analyst) - [Focus: SOC Operations & Detection]
* **13Cubed** Windows Memory Analysis - [Focus: DFIR Deep Dive]
* [Upcoming] **TCM Security PMRP** (Practical Malware Research Professional)
* [Upcoming] **MAD20** Threat Hunting and Detection Engineering

### 📅 Future Objectives

#### 2027: Offensive & AD Mastery
* **CRTP** (Certified Red Team Professional)
* **CRTO** (Certified Red Team Operator)
* **CREST CPTIA**

#### 2028: Expert Level Penetration Testing
* **CPTS** (Certified Penetration Testing Specialist)
* **OSCP** (Offensive Security Certified Professional)

### 🌟 Advanced Specialization (Employer-Sponsored Goals)
*These elite certifications represent my commitment to mastering industry-leading standards in senior-level roles.*

* **GCFA** (GIAC Certified Forensic Analyst): Advanced incident response and threat hunting.
* **GCTI** (GIAC Cyber Threat Intelligence): Strategic and tactical threat intelligence mastery.
* **GDAT** (GIAC Defeating Advanced Adversaries): The ultimate Purple Team validation – integrating detection, response, and adversary emulation.

</details>

---

*Maintained by Juana | Cyber Security Analyst* *Last Updated: March 2026*