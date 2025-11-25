# My Malware Analysis Lab & PMAT Notes

![Category](https://img.shields.io/badge/Category-Malware%20Analysis-red)
![Status](https://img.shields.io/badge/Status-Learning%20%2F%20In%20Progress-yellow)

Welcome to my malware analysis repository! 👋

This project documents my journey through the **Practical Malware Analysis & Triage (PMAT)** course by **TCM Security**. It contains my personal study notes, resources, and configuration guides for building a safe analysis environment.

> **Current Status**: 🌱 **Early Learning Stage**
> I am currently focused on establishing a robust, isolated laboratory environment and organizing essential tooling.

## 📂 Current Contents

While the course recommends VirtualBox, I have opted to build an enterprise-grade lab using **XCP-ng (Bare-metal Hypervisor)**.

### 1. Lab Setup Guide
This is the primary documentation in this repository. It details my custom approach to deploying a malware lab from scratch using XCP-ng.
- **[📄 Read: Malware Analysis Lab Setup with XCP-ng](Environment/Malware%20Analysis%20Lab%20Setup%20with%20XCP-ng.md)**
    - **Highlights**: Features a **pfSense** controller for strict network isolation ("Dirty Line"), **REMnux** (Analysis Node), and **FlareVM** (Victim Node).
    - **Topics Covered**: Hardware requirements, Dom0 tuning, VLAN isolation, the pfSense "Kill Switch", and mitigations for anti-VM detection.

### 2. Tools & Resources
A consolidated reference list of tools used throughout the PMAT course, along with safe sources for malware samples.
- **[📄 Read: PMAT Tools List & Download Resources](Resources/PMAT%20Tools%20List%20&%20Download%20Resources.md)**

---

## ⚠️ Disclaimer

**Please Read Carefully:**

1.  **Safety First**: This repository discusses handling live malware. All practical exercises must be performed inside a strictly isolated virtual machine (Sandbox). **NEVER** run malware samples on your host machine or production network.
2.  **Educational Purpose**: The contents of this repository are for educational and defensive research purposes only. The author is not responsible for any misuse of the information provided.
3.  **Personal Notes**: These are my personal study notes and are not a replacement for the official course materials.

---

## 🙏 Credits & Acknowledgments

The methodology and learning path in this repository are derived from the excellent **Practical Malware Analysis & Triage (PMAT)** course by **HuskyHacks**.

* **Course Author**: HuskyHacks (@HuskyHacks)
* **Course Link**: [Practical Malware Analysis & Triage @ TCM Security](https://academy.tcm-sec.com/p/practical-malware-analysis-triage)

If you find these notes useful, I highly recommend purchasing the full course to support the creator.

---

*Last Updated: 2025*
