# Day 24 – Module 12: Evading IDS, Firewalls, and Honeypots

## 🔥 What is a Firewall?
A firewall is a **network security device or software** that monitors and filters incoming and outgoing network traffic based on an organization’s previously established security policies.

### 🔐 Types of Firewalls:
1. **Packet-Filtering Firewall** – Filters traffic based on IP addresses, ports, and protocols.
2. **Stateful Firewall** – Tracks the state of active connections and determines which packets are part of a valid connection.
3. **Stateless Firewall** – Analyzes individual packets without context.
4. **Deep Packet Inspection (DPI)** – Examines the data and header content of each packet.

### 🔍 Firewall Filtering Techniques:
- **Signature-Based Filtering**
- **Behavior-Based Filtering**
- **Header-Based Filtering**

### 🧱 Deployment Types:
- **Software Firewall** – Runs as an application on a device (e.g., Windows Defender Firewall).
- **Hardware Firewall** – A physical appliance for perimeter defense.

---

## 🛡️ Web Application Firewall (WAF)

A **WAF** is a specialized firewall that filters, monitors, and blocks HTTP traffic to and from a web application. It helps protect against attacks such as:
- Cross-site Scripting (XSS)
- SQL Injection
- File Inclusion
- Session Hijacking

### 🧪 Tool Used for WAF Detection:
- `wafw00f` – A Python tool used to identify the presence and type of WAF protecting a website.

---

## 🕵️‍♂️ What is IDS (Intrusion Detection System)?

An **IDS** is a security mechanism that monitors network or system activity for malicious actions or policy violations.

### 🧠 How IDS Detects Intrusions:
- Signature-Based Detection  
- Anomaly-Based Detection  
- Protocol Anomaly-Based Detection
- Heuristic-Based Detection  

### 📊 Types of IDS:
1. **Network-Based IDS (NIDS)** – Monitors entire network traffic.
2. **Host-Based IDS (HIDS)** – Monitors a single host for suspicious activity.

### ⚠️ Types of IDS Alerts:
- **True Positive** – Actual attack correctly detected
- **False Positive** – Normal activity flagged as attack
- **True Negative** – Normal activity correctly not flagged
- **False Negative** – Attack not detected

---

## 🪤 What are Honeypots?

A **Honeypot** is a **deceptive system or resource** designed to be attacked or compromised, providing security professionals insight into attacker behavior and methods.

### 🧱 Types of Honeypots:
1. **Low-Interaction Honeypots** – Simulate limited services (e.g., ports, banners).
2. **High-Interaction Honeypots** – Full OS and services for deeper observation.
3. **Client Honeypots** – Emulate client-side environments to attract client-targeted attacks.

### 🛠️ Honeypot Tools:
- **Snort** – Can function as IDS and honeypot
- **Pentbox** – Lightweight security toolkit with honeypot functionality
- **HoneyBOT** – Windows-based honeypot simulator
- **Valhalla** – Advanced honeypot focused on malware collection

---

## 📝 Summary:

On **Day 24**, I studied **Module 12: Evading IDS, Firewalls, and Honeypots**. The session covered **various defensive technologies**, how attackers try to evade them, and the tools used for both detection and deception. I learned the roles and architectures of **firewalls, IDS, WAFs**, and **honeypots**, along with practical tools like `wafw00f`, `snort`, and `pentbox`. Understanding these defenses is critical in developing effective **evasion strategies and countermeasures**.

---
