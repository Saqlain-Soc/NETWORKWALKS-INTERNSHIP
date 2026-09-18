
# 🔎 NETWORK SCANNING REPORT

![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity-blue)
![Zenmap](https://img.shields.io/badge/Tool-Zenmap-red)
![Windows](https://img.shields.io/badge/Platform-Windows-0078D6)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

Network Scanning & Host Discovery with Zenmap

*WEEK 02 | PM5 | NETWORK SCANNING WITH ZENMAP*

---

## 🔹 Assessment Overview

| **Field** | **Details** |
| :--- | :--- |
| 👨‍💻 **Intern** | **Saqlain Abbas** |
| 🎓 **Program / Batch** | **NETWORKWALKS Cybersecurity Internship** |
| 🧪 **Module** | **Week 02 — PM5: Network Scanning with Zenmap** |
| 🎯 **Target Subnet** | **192.168.80.0/24 (VMware VMnet8 NAT)** |
| 🔐 **Authorization** | ✅ **Authorized Internship Task** |
| 🛰️ **Phase** | **Scanning & Network Discovery** |
| 📌 **Assessment Type** | **Authorized Network Reconnaissance** |
| ✅ **Status** | **Completed** |

---

## 1. ⚠️ Liability Disclaimer

All activities were performed for educational purposes on my own local VMware NAT network (`192.168.80.0/24`), which is entirely under my control. No external or unauthorized networks were scanned.

---

## 2. 📖 Introduction

This report covers network scanning and host discovery using **Zenmap** (the GUI for Nmap) as part of Week 02 of the NETWORKWALKS Cybersecurity Internship. The objective was to install Zenmap on Windows, identify the local subnet, and perform authorized host discovery to identify active devices on the network.

---

## 🛠️ 3. Tools Used

| **Tool** | **Purpose** |
| :--- | :--- |
| 💻 **Windows CMD** | Identify local network configuration |
| 🛰️ **Zenmap (Nmap GUI)** | Discover live hosts and network devices |

---

## 🖥️ 4. Lab Environment

| **Component** | **Details** |
| :--- | :--- |
| Host OS | Windows |
| Hypervisor | VMware Workstation |
| Network | VMware VMnet8 NAT |
| Subnet | 192.168.80.0/24 |
| Gateway | 192.168.80.1 |
| Kali Linux IP | 192.168.80.131 |

---

## 🔍 5. Tasks Completed

### 5.1 — Zenmap Installation

Zenmap was downloaded from the official source ([nmap.org/download.html](https://nmap.org/download.html)) and installed successfully on Windows.

---

### 5.2 — Local IP & Subnet Identification

**Command executed:**
```cmd
ipconfig
```

**Result:**

| **Field** | **Value** |
| :--- | :--- |
| VMware Network Adapter | VMnet8 → 192.168.80.1 |
| Subnet Mask | 255.255.255.0 |
| Target Subnet | 192.168.80.0/24 |

**📸 Evidence:** `01-ipconfig.png`

---

### 5.3 & 5.4 — Live Host Discovery

| **Field** | **Value** |
| :--- | :--- |
| Target | 192.168.80.0/24 |
| Profile | Ping scan |
| Command | `nmap -sn 192.168.80.0/24` |
| Live Hosts Found | **3** |

**📸 Evidence:** `02-zenmap-ping-scan.png` · `Output.png`

---

### 5.5 — IP Addresses of Live Hosts

| **IP Address** | **Role** |
| :---: | :--- |
| `192.168.80.1` | Gateway / Host |
| `192.168.80.131` | Kali Linux VM |
| `192.168.80.254` | VMware Virtual Host |

---

### 5.6 — MAC Addresses of Live Hosts

| **IP Address** | **MAC Address** | **Vendor** |
| :---: | :---: | :--- |
| `192.168.80.131` | 00:0C:29:71:83:FF | VMware |
| `192.168.80.254` | 00:50:56:FF:90:18 | VMware |
| `192.168.80.1` | (Gateway) | — |

**📸 Evidence:** `03-hosts-list.png` · `Output.png`

---

### 5.7 — Network Topology

The Topology view was generated and saved as PDF.

**📸 Evidence:** `04-topology.png` · `Topology.pdf`

---

## 📊 6. Summary

| **Item** | **Result** |
| :--- | :--- |
| Live Hosts | 3 |
| Live IPs | 192.168.80.1, .131, .254 |
| Scan Duration | ~9.82 seconds |
| Topology Saved | ✅ Yes (PDF) |

---

## 🧠 7. Key Learnings

* Zenmap makes Nmap easier to use through a **graphical interface**.
* Ping scan (`-sn`) is useful for **quick host discovery** without port scanning.
* MAC addresses help identify **virtual machines** (VMware vendor prefixes).
* Topology view gives a **visual map** of the network layout.
* Scanning should always be limited to **your own authorized lab network**.

---

## ✅ 8. Conclusion

During Week 02 of the NETWORKWALKS Cybersecurity Internship, I used Zenmap/Nmap to perform network discovery on my local VMware NAT subnet. The scan identified **3 live hosts** and provided details such as IP addresses, MAC addresses, and network topology. This practical strengthened my understanding of **host discovery, network mapping, and the scanning phase** of an authorized security assessment.

---

## 📊 9. Project Summary

| **Category** | **Details** |
| :--- | :--- |
| **Project** | NETWORKWALKS Internship — Week 02, PM5 |
| **Focus** | Network Scanning & Host Discovery |
| **Tool** | Zenmap / Nmap |
| **Target Network** | 192.168.80.0/24 |
| **Live Hosts Identified** | **3** |
| **Status** | **Completed** |

---

## 👤 Author

### Saqlain Abbas

**🔐 Cybersecurity Intern — NETWORKWALKS**

> `Learning → Building → Testing → Securing`

This repository forms part of my practical cybersecurity internship portfolio and documents my hands-on laboratory exercises.

<p align="center">
  <a href="https://linkedin.com/in/saqlain-abbas-a61b59414">
    <img src="https://img.shields.io/badge/🔵_LinkedIn-Professional%20Profile-0A66C2?style=for-the-badge" />
  </a>
  &nbsp;
  <a href="https://github.com/Saqlain-Soc">
    <img src="https://img.shields.io/badge/⚫_GitHub-Security%20Projects-181717?style=for-the-badge" />
  </a>
</p>

---
