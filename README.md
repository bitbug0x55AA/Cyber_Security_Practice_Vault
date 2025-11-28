# Malware Analysis & Reverse Engineering Portfolio

![Category](https://img.shields.io/badge/Category-Malware%20Analysis%20%26%20Reverse%20Engineering-red)
![Status](https://img.shields.io/badge/Status-Active%20Learning-blue)
![Focus](https://img.shields.io/badge/Focus-Lab%20Reports%20%26%20Practical%20Output-success)

Welcome to my malware analysis portfolio! 👋

This repository was originally initialized to document my progress through the **PMAT** course. However, my objectives have evolved into building a comprehensive skill tree in **Malware Analysis** and **Reverse Engineering**.

Consequently, this project now serves as a dedicated portfolio to archive my **practical outputs**, including engineering documentation for lab infrastructure, detailed analysis reports of malware samples, and reverse engineering exercises. It aims to document the journey from basic triage to advanced automation.

## 🗺️ Roadmap & Learning Path

My learning path follows a structured progression from foundational analysis to low-level architecture, and finally to advanced reverse engineering and automation.

| Stage | Course / Resource | Provider | Status | Focus |
| :--- | :--- | :--- | :--- | :--- |
| **01** | **Practical Malware Analysis & Triage (PMAT)** | TCM Security | 🟡 **In Progress** | Basic Static/Dynamic Analysis, Network Signatures, Report Writing |
| **02** | **Architecture 1001: x86-64 Assembly** | OpenSecurityTraining2 | ⚪ *Planned* | Assembly Language, Low-level Computer Architecture |
| **03** | **Zero2Hero Bootcamp** | Independent | ⚪ *Planned* | Malware Development Techniques, Advanced PE Structure, Evasion |
| **04** | **Zero2Automated** | OALabs | ⚪ *Planned* | Advanced Reverse Engineering, Deobfuscation, Config Extraction |

## 📂 Repository Contents

This repository is strictly for engineering outputs and lab reports.

### 1. Lab Infrastructure (Engineering)
Documentation on building and maintaining an enterprise-grade analysis environment. I have opted to use **XCP-ng (Bare-metal Hypervisor)** instead of standard desktop virtualization to simulate a realistic, air-gapped network.
- **[📄 Read: Malware Analysis Lab Setup with XCP-ng](Environment/Malware%20Analysis%20Lab%20Setup%20with%20XCP-ng.md)**
    - **Highlights**: Features a pfSense "Dirty Line" architecture, REMnux (Controller), FlareVM (Victim), and hardware-level anti-VM evasion hardening.

### 2. Analysis Reports (Lab Practice)
Detailed reports derived from analyzing real-world or simulated malware samples. Each report includes extracted IOCs, behavioral analysis, and reverse engineering findings.
- **Sample Reports**:
    - [x] [Basic Static Analysis: Malware.Unknown.exe](Lab%20Practice/1-1.%20Basic-Static-Analysis-Practice-01.md)
    - [ ] *Advanced Dynamic Analysis (Coming Soon)*
    - [ ] *Unpacking & Deobfuscation (Coming Soon)*

### 3. Tooling & Resources
A consolidated reference list of the toolsets used throughout this learning path, along with vetted sources for obtaining safe malware samples.
- **[📄 Read: Tools List & Download Resources](Resources/Tools%20List%20&%20Download%20Resources.md)**

---

## ⚠️ Disclaimer

**Please Read Carefully:**

1.  **Safety First**: This repository contains references to and analysis of **live malware**. All practical exercises documented here were performed inside a strictly isolated, air-gapped virtualization environment. **NEVER** run malware samples on your host machine or production network.
2.  **Educational Purpose**: The contents of this repository are for educational and defensive research purposes only. The objective is to understand threat behaviors to better defend against them.
3.  **No Liability**: The author is not responsible for any damage caused by the misuse of the information or code provided in this repository.

---

## 🙏 Acknowledgments & Credits

Special thanks to the creators of the high-quality training materials that guide this path:

* **HuskyHacks** (@HuskyHacks) - for the foundational *PMAT* course.
* **XenoKovah** (@XenoKovah) - for the *OpenSecurityTraining2* architecture courses.
* **Vitali Kremez & 0verfl0w_** - for the advanced *Zero2Automated* content.

---

*Last Updated: 2025*