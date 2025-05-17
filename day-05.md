# 📅 Day 05 – Module 3: Scanning

## 📘 Topics Covered
- What is Scanning?
- Footprinting vs. Scanning
- Types of Scanning
- Objectives of Scanning
- Understanding Ports and Port Types
- Three-Way Handshake
- TCP Flags and Their Functions
- Scanning Tools (CLI & GUI)
- Nmap Usage and Command Examples
- MITRE ATT&CK Framework

---

## 🔍 What is Scanning?

Scanning is the second phase in the hacking methodology, where attackers interact with target systems to discover open ports, services, live hosts, and potential vulnerabilities.

> ⚠️ *Footprinting is passive (no interaction), whereas Scanning is active (direct interaction with the system).*

---

## 🧭 Objectives of Scanning
- Detect live systems (ping sweep)
- Discover open ports and services
- Identify operating systems and their versions
- Detect vulnerabilities or misconfigurations

---

## 🔌 Ports and Their Types

### 📦 Physical Ports
- Hardware interfaces (e.g., USB, HDMI)

### 🌐 Logical Ports (Used in Networking)
- **Well-Known Ports**: 0–1023 (e.g., HTTP - 80, HTTPS - 443, FTP - 21)
- **Registered Ports**: 1024–49151
- **Dynamic/Private Ports**: 49152–65535

---

## 🤝 TCP Three-Way Handshake

Essential for establishing a TCP connection:

1. **SYN** → Initiate a connection
2. **SYN-ACK** → Acknowledge receipt
3. **ACK** → Finalize connection

---

## 🚩 TCP Flags
| Flag  | Description                       |
|-------|-----------------------------------|
| URG   | Urgent pointer field significant  |
| ACK   | Acknowledgment field significant  |
| PSH   | Push function                     |
| RST   | Reset the connection              |
| SYN   | Synchronize sequence numbers      |
| FIN   | No more data from sender          |

---

## 🛠️ Scanning Tools

### 🖥️ Command Line Tools
- **Nmap** – Versatile and powerful scanner  
- **RustScan** – Faster alternative to Nmap for port discovery  
- **Metasploit (msfconsole)** – Integrated scanning and exploitation  
- **enum4linux** – SMB/NetBIOS enumeration  

### 🧰 GUI Tools
- **Zenmap** – Nmap with a GUI frontend  
- **Angry IP Scanner** – Quick live host detection  

---

## 🔎 Nmap Commands (Basics)

```bash
nmap -sS <target>         # TCP SYN scan (stealth)
nmap -sT <target>         # TCP connect scan
nmap -sU <target>         # UDP scan
nmap -O <target>          # OS detection
nmap -sV <target>         # Service/version detection
nmap -p- <target>         # Scan all 65535 ports
nmap -A <target>          # Aggressive scan (OS, version, script, traceroute)
```

- nmap cheetsheet - https://www.stationx.net/nmap-cheat-sheet/

---

## 🧬 MITRE ATT&CK Framework

MITRE ATT&CK is a globally accessible knowledge base of adversary tactics and techniques based on real-world observations.

### 🧠 Key Concepts:
- Tactics – Goals of an attacker (e.g., initial access, lateral movement)
- Techniques – How the attacker achieves those goals
- Sub-techniques – More specific implementations
- Use Case – Maps scanning activities to tactics like Discovery, Reconnaissance, etc.

## 📌 Summary
Day 5 - Learned about the active nature and objectives of scanning. Explored key networking concepts like ports, TCP flags, and scanning types. Hands-on exposure to scanning tools and basic nmap usage. Introduction to the industry-grade MITRE ATT&CK framework. 

>  *📈 Takeaway: Scanning bridges the gap between passive intelligence gathering (footprinting) and active vulnerability exploitation. It's a critical phase in ethical hacking and red teaming.*
