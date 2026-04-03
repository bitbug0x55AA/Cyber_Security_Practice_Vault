# Lab Infrastructure & Environment

> Central repository for home lab architecture, network segregation policies, and virtual machine inventory.

## 🗺️ Logical Network Topology

The lab environment is virtually hosted on a Mini PC running **XCP-ng**. Network routing and segregation are strictly enforced by a **pfSense** virtual appliance, dividing the environment into three core zones:

* **Zone 1: WLAN (Home/Management Network)**
    * Trusted zone. Houses management interfaces, SIEM aggregators, and containerized threat intelligence pipelines.
* **Zone 2: LAN (DFIR & Malware Analysis)**
    * Restricted zone. Dedicated to malware detonation and forensic artifact processing. 
* **Zone 3: Adversary (Emulation Range)**
    * Isolated range. Hosts the attack infrastructure and vulnerable target machines for end-to-end emulation.

## Telemetry & Data Flow Pipeline

To strictly manage VM resource consumption and respect SIEM license constraints (e.g., Splunk daily ingestion limits), this lab employs an **On-Demand Offline Telemetry Pipeline** rather than continuous network log forwarding:

1. **Local Acquisition**: Raw event logs (EVTX) and artifacts are manually collected from target endpoints post-emulation.
2. **Offline Parsing**: Artifacts are processed using `EvtxECmd` to generate highly structured JSON outputs.
3. **Ad-Hoc Ingestion**: Parsed JSON files are manually uploaded to the Splunk instance (WLAN) for isolated hunting and analysis.
4. **Environment Rollback**: Post-analysis, the SIEM instance and target VMs are immediately rolled back to a clean state to flush the indexed data and reset the license counter.

*Note: This architecture mimics dead-box DFIR workflows and ensures that no inbound firewall ports need to be opened from the compromised zones (LAN/Adversary) to the trusted management zone (WLAN).*

## Infrastructure Sub-Domains

* **`XCP-ng_Base_Setup/`**: Foundational hypervisor configurations, pfSense firewall rules, and snapshot management policies.
* **`Active_Directory_Ranges/`**: Configurations and vulnerable deployment states for the Windows Server domain environment.
* **`Docker_and_Tooling/`**: Docker Compose files for services hosted on the management MacBook (Elastic SIEM, FreshRSS CTI Streamer).

---

## Virtual Machine & Service Inventory

The following table tracks the active staging, monitoring, and detonation targets currently provisioned within the infrastructure.

### 1. Trusted Management & Monitoring (WLAN)

| Hostname / Service | OS / Platform | Primary Role | Segment | Notes |
| :--- | :--- | :--- | :--- | :--- |
| `XOA` | Appliance | Xen Orchestra Management | WLAN | Controls VM lifecycle and snapshots. |
| `SIEM-SPLUNK` | Ubuntu Server | Log Aggregation (Splunk) | WLAN | Operates on an ad-hoc ingestion model. Rolled back after each hunting session. |
| `MAC-DOCKER-SIEM` | macOS (Docker) | Elastic SIEM | WLAN | Lightweight alternative SIEM testing instance. |
| `MAC-DOCKER-CTI` | macOS (Docker) | FreshRSS CTI Streamer | WLAN | Automated threat intelligence feed aggregation. |

### 2. Analysis & Forensics Range (LAN)

| Hostname | OS / Platform | Primary Role | Segment | Notes |
| :--- | :--- | :--- | :--- | :--- |
| `WIN-FLARE` | Windows 10/11 | Malware Detonation & DFIR | LAN | Dual-purpose analysis box. Reverted to clean snapshot post-detonation. |
| `REMNUX-01` | Ubuntu 20.04 | Network Simulator / Toolkit | LAN | Used intermittently with FlareVM for network traffic analysis and simulation. |

### 3. Adversary Emulation Range (Adversary)

| Hostname | OS / Platform | Primary Role | Segment | Notes |
| :--- | :--- | :--- | :--- | :--- |
| `KALI-ATTACK` | Kali Linux | Adversary Infrastructure | Adversary | Staging ground for offensive tools and C2 frameworks. |
| `DC-CORP-01` | Windows Server 2019 | Target Domain Controller | Adversary | Vulnerable endpoint for Active Directory exploitation and artifact generation. |

---
*Note: Passwords and specific IP addresses are omitted from this public-facing document. The environment is physically and logically isolated from any production infrastructure.*