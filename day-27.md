# Day 27 – Module 5: Vulnerability Analysis

## 🛡️ What is Vulnerability Assessment?
Vulnerability Assessment (VA) is the process of **identifying, classifying, and prioritizing security vulnerabilities** in systems, networks, and applications. It is a foundational step in proactive cybersecurity to reduce risk and improve overall posture.

---

## 📂 Types of Vulnerabilities

### 🆔 CVE – Common Vulnerabilities and Exposures
A publicly disclosed database of known vulnerabilities, each assigned a unique CVE ID (e.g., CVE-2023-12345).

### 🧱 CWE – Common Weakness Enumeration
A community-developed list of software and hardware **weaknesses or flaws**, such as buffer overflows, SQL injection, etc.

### 📊 CVSS – Common Vulnerability Scoring System
A framework for rating the severity of vulnerabilities:
- **Scores range from 0.0 (None) to 10.0 (Critical)**
- Considers exploitability, impact, and environmental factors

### 🌐 NVD – National Vulnerability Database
A U.S. government repository of standards-based vulnerability data, built upon CVE and enriched with **CVSS scores**, patch data, and impact analysis.

---

## 🧰 Practical Exercise: Nessus Essentials on Kali Linux

### 🔽 Nessus Installation:
- Downloaded **Nessus Essentials** from [download link](https://www.tenable.com/products/nessus/nessus-essentials)
- Installed and activated it on **Kali Linux** using the registration code provided by Tenable
- Accessed the Nessus Web Interface via:  
  `https://localhost:8834`

### 🧪 Conducted a Vulnerability Scan:
- **Target**: `testphp.vulnweb.com`
- Created a **basic scan profile**
- Launched the scan and reviewed the report:
  - Discovered **high, medium, and low severity vulnerabilities**
  - Exported the scan results for internal analysis

📌 *Note: All scanning was conducted on intentionally vulnerable test environments, strictly for educational purposes.*

---

## 🤖 Bonus Tip: Introduction to tgpt

At the end of the session, our mentor introduced **tgpt**, a **terminal-based ChatGPT CLI tool** that allows command-line interactions with AI. However, it was emphasized that:

> "Students must first practice and understand manual methodologies before relying on AI tools like tgpt."

This aligns with the ethical and pedagogical goal of building **core competencies** in real-world cybersecurity before enhancing workflows with automation and AI.

---

## 📝 Summary:

On **Day 27**, I completed **Module 5: Vulnerability Analysis**. The session provided a solid foundation on **vulnerability identification frameworks** (CVE, CWE, CVSS, NVD) and introduced **Nessus Essentials** for hands-on scanning of test environments. The concept of using **tgpt** was introduced as a supplementary aid, but manual skill-building remains the priority in ethical hacking practices.

---
