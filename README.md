# 🛡️ CEH v13 Notes by 10ayy
Welcome to my **Certified Ethical Hacker(CEHv13)** study notes repository.

This repository contains my day-wise notes from the **Certified Ethical Hacker (CEH v13)** training. It includes key concepts, tools, commands, and practical exercises that I am learning as I progress through the official CEH course.

---

## 📌 Objective

- Maintain structured, consistent documentation of my daily learning.
- Reinforce knowledge through note-taking and practical command usage.
- Create a public knowledge base to help myself and others revising CEH.
- At the end of my course, I will convert these notes into a **comprehensive Document/PDF**.

---

## 📂 Repository Structure
```bash
CEH-Notes/
|   
├── README.md
├── day-01.md
├── day-02.md
├── day-03.md
├── day-04.md
├── day-05.md
├── day-06.md
├── day-07.md
├── day-08.md
├── day-09.md
├── day-10.md
├── day-11.md
├── day-12.md
├── day-13.md
├── day-14.md
├── day-15.md
├── day-16.md
├── day-17.md
├── day-18.md
├── day-19.md
├── day-20.md
├── day-21.md
├── day-22.md
├── day-23a.md
├── day-23b.md
├── day-24.md
├── day-25.md
├── day-26a.md
├── day-26b.md
├── day-27.md
├── day-28.md
└── lab-setup.md
```

---

## 🧪 Lab Setup

A detailed guide to setting up your own isolated CEH virtual lab using VMware/VirtualBox is available here → [Lab Setup](lab-setup.md)

This setup includes:

- Attacker Machine: Kali Linux / Parrot OS

- Victim Machines: Metasploitable 2 and Windows 10

- Networking: Host-only or NAT for isolated testing

---

## 📅 Course Progress Tracker

| Day | Module            | Topics Covered                                            | Link                         |
|-----|-------------------|-----------------------------------------------------------|------------------------------|
| 01  | Module 01          | Introduction to Ethical Hacking                           | [Day 01 Notes](day-01.md)    |
| 02  | Module 01          | Cybersecurity Terminologies, CIA, Laws                    | [Day 02 Notes](day-02.md)    |
| 03  | Module 02          | Footprinting & Reconnaissance (Intro)                     | [Day 03 Notes](day-03.md)    |
| 04  | Module 02          | Footprinting Tools & Google Dorking                       | [Day 04 Notes](day-04.md)    |
| 05  | Module 03          | Scanning - Ports, Protocols, and Nmap                     | [Day 05 Notes](day-05.md)    |
| 06  | Module 04          | Enumeration (Intro, FTP, SSH, Practical Access)           | [Day 06 Notes](day-06.md)    |
| 07  | Module 04          | Enumeration (SMB, SNMP, LDAP, SMTP, Tools)                | [Day 07 Notes](day-07.md)    |
| 08  | Module 07          | Malware Threats (Theory)                                  | [Day 08 Notes](day-08.md)    |
| 09  | Module 07          | Malware Threats  (Reverse Shell via Malware)              | [Day 09 Notes](day-09.md)    |
| 10  | Module 06          | System Hacking                                            | [Day 10 Notes](day-10.md)    |
| 11  | Practical         | TryHackMe Practical Lab                                   | [Day 11 Notes](day-11.md)    |
| 12  | Practical         | TryHackMe Practical Lab, CrackTheLab                      | [Day 12 Notes](day-12.md)    |
| 13  | Module 08          | Sniffing                                                  | [Day 13 Notes](day-13.md)    |
| 14  | Module 09          | Social Engineering                                        | [Day 14 Notes](day-14.md)    |
| 15  | Module 10         | Denial-of-Service                                         | [Day 15 Notes](day-15.md)    |
| 16  | Module 11         | Session Hijacking                                         | [Day 16 Notes](day-16.md)    |
| 17  | Module 14         | Hacking Web Application                                   | [Day 17 Notes](day-17.md)    |
| 18  | Module 14         | Hacking Web Application (Practical: DVWA)                 | [Day 18 Notes](day-18.md)    |
| 19  | Practical         | TryHackMe Practical Lab                                   | [Day 19 Notes](day-19.md)    |
| 20  | Module 13         | Hacking Web Servers (Theory + Practical: DVWA)            | [Day 20 Notes](day-20.md)    |
| 21  | Module 15         | SQL Injection                                             | [Day 21 Notes](day-21.md)    |
| 22  | Practical         | TryHackMe Practical Lab and PortSwigger Introduction      | [Day 22 Notes](day-22.md)    |
| 23  | Module 18         | IoT Hacking                                               | [Day 23a Notes](day-23a.md)    |
| 23  | Module 19         | Cloud Computing                                           | [Day 23b Notes](day-23b.md)    |
| 24  | Module 12         | Evading IDS, Firewalls and Honeypots                      | [Day 24 Notes](day-24.md)    |
| 25  | Module 20         | Cryptography                                              | [Day 25 Notes](day-25.md)    |
| 26  | Module 17         | Hacking Mobile Platforms                                  | [Day 26a Notes](day-26a.md)    |
| 26  | Module 16         | Hacking Wireless Networks                                 | [Day 26b Notes](day-26b.md)    |
| 27  | Module 05         | Vunlerability Analysis                                    | [Day 27 Notes](day-27.md)    |
| 28  | Module 16         | Hacking Wireless Networks(Practical)                      | [Day 28 Notes](day-28.md)    |

> ✅ *More updates coming as I progress in the course.*

---

## 🧠 Tools Covered So Far

- **CLI-Based**: `nmap`, `nslookup`, `dig`, `theHarvester`, `enum4linux`, `rustscan`, `msfconsole`, `whois`, `subfinder`, `dirb`, `gobuster`, `dnsrecon`, `dmitry`, `nbtstat`, `enum4linux`, `smbclient`, `snmpwalk`, `ntptrace`, `telnet`, `Nmap scripts`, `hydra`, `msfvenom`, `hydra`, `ettercap`, `bettercap`, `macchanger`, `macof`, `yersinia`, `zphisher`, `setoolkit`, `camphish`, `goldeneye`, `sqlmap`, `netcat`, `HoneyBot`, `pentbox`, `wafw00f`, `md5sum`, `hashcalc`, `cyberchef`, `cryptr`, `hashcat`, `john`, `veracrypt`, `tgpt`, `airmon-ng`, `airocrack-ng`, `airplay-ng`
- **GUI-Based**: `Zenmap`, `Angry IP Scanner`, `Wappalyzer`, `Hunter.io`, `Netcraft`, `Shodan`, `Censys`, `dnsdumpster.com`, `Technitium`, `base64topdf`, `CyberChef`, `CookieEditor`, `FoxyProxy`, `wireshark`, `BurpSuite`, `Snort`, `Valhala`, `crackthestation.com`, `Base64.com`, `mdshashgenerator`, `AhMyth`, `Nessus Essentials`

---

## 🗃️ Contribution & Feedback 
This repo is a personal knowledge base, but suggestions, corrections, and feedbacks are welcome.

Feel free to reach out via issues or LinkedIn!!!

---

## ⚠️ Disclaimer

This repository is for **educational purposes only**. All the tools and techniques discussed are meant for lawful, ethical, and academic use.

---

## 📫 Connect with me

[LinkedIn] https://www.linkedin.com/in/tanay-wasnik-59b49323b/

[GitHub] https://github.com/10ayy/
