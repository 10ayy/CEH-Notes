# Day 19 – Practical Labs: Passive Reconnaissance & Phishing Analysis

## 🧪 Labs Covered on TryHackMe

Today, two practical labs were solved under guided supervision to reinforce the theoretical and practical understanding of **passive reconnaissance** and **phishing attack analysis**.

---

## 🧭 Lab 1: Passive Recon (TryHackMe)

**Room**: [Passive Recon](https://tryhackme.com/room/passiverecon)

### 🧠 Key Learnings:
- Understood the **importance of passive information gathering** in the early stages of penetration testing.
- Explored various passive reconnaissance techniques to identify:
  - WHOIS records
  - DNS records
  - Publicly available metadata
  - Subdomains and archived data using **tools like crt.sh, Wayback Machine, Shodan, Censys**, etc.
- Used **Google Dorking** for intelligent search queries to extract sensitive data unintentionally exposed on the internet.

### 🔧 Tools & Techniques:
- [crt.sh](https://crt.sh/)
- [Wayback Machine](https://archive.org/web/)
- [Google Dorks](https://www.exploit-db.com/google-hacking-database)
- [Shodan](https://www.shodan.io/)
- [Censys](https://search.censys.io/)
- WHOIS Lookup tools (whois.domaintools.com, ICANN)

---

## 🛡️ Lab 2: Phishing Analysis Fundamentals (TryHackMe)

**Room**: [Phishing Analysis Fundamentals](https://tryhackme.com/room/phishinganalysisfundamentals)

### 🧠 Key Learnings:
- Understood the **mechanism of phishing emails**, and how to dissect and analyze them.
- Identified malicious indicators in:
  - Email headers
  - Attachments (suspicious macros, scripts)
  - URLs and shortened links
- Analyzed phishing payloads (e.g., malicious Office documents or PDFs) and behavior post-execution.
- Gained insights into how **social engineering and phishing** are often the **initial access vectors** in real-world cyberattacks.

### 🔧 Tools & Techniques:
- Email header analysis via **MxToolbox** or **base64topdf**
- URL decoding & expansion
- Office document macro inspection
- Basic static and behavioral analysis of attachments

---

## 📝 Summary:

On Day 19, two essential **reconnaissance and incident analysis labs** were solved from TryHackMe:
1. **Passive Recon** demonstrated the significance of non-intrusive intel gathering during the pre-attack phase. 
2. **Phishing Analysis Fundamentals** taught how to analyze phishing emails and detect potential compromise vectors.

These practicals further solidified our understanding of **OSINT techniques and social engineering tactics**, crucial in both offensive and defensive cybersecurity domains.

---
