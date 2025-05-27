# Day 11 – Practical Application: TryHackMe Room – "Library"

## 🧪 Practical Module: Applying Scanning & Enumeration Techniques

On Day 11, I applied theoretical knowledge from previous modules in a hands-on **penetration testing scenario** using the [TryHackMe](https://tryhackme.com/) platform. The room completed was **"Library"**, a beginner-intermediate level CTF room focused on service enumeration, directory discovery, brute-forcing, and privilege escalation.

---

## 🛠️ Tools Utilized

- **Nmap** – For port and service discovery
- **Gobuster** – For directory enumeration
- **Hydra** – For brute-forcing SSH credentials
- **OpenSSH** – For gaining shell access

---

## 🔍 Step-by-Step Walkthrough

### 1. 🔎 Port Scanning with Nmap

Performed a full scan to identify open ports and running services:

```bash
nmap -sC -sV -oN library-nmap.txt <target-IP>
```
Identified key open ports:
- 22/tcp – OpenSSH
- 80/tcp – HTTP service hosting a basic website

### 2. 🕸️ Web Enumeration

Visited the website(target-ip) on port 80. From the homepage, extracted:
- A potential username
- Hints towards hidden directories

### 3. 📂 Directory Brute-Forcing with Gobuster

Used Gobuster to uncover hidden subdirectories:

```bash
gobuster dir -u http://<target-IP> -w /usr/share/wordlists/dirb/common.txt
```
Discovered a few directories which helped identify the system structure and confirmed the presence of a login interface.

### 4. 🔐 SSH Brute Force with Hydra

Based on the username identified earlier, used Hydra to brute-force the SSH credentials:

```bash
hydra -l <username> -P /usr/share/wordlists/rockyou.txt ssh://<target-IP>
```
> Successfully obtained valid SSH credentials.

### 5. 🔑 Gaining Access via SSH

Logged into the system using SSH:

```bash
ssh <username>@<target-IP>
```

Located the user flag:

```bash
cat user.txt
```

✅ User flag captured successfully.

---

## ⬆️ Root Privilege Escalation (Pending)

The `root.txt` flag is currently inaccessible due to restricted privileges. This will be addressed in a future session focused on privilege escalation techniques and root access strategies.

---

## 📝 Summary

Day 11 was a practical application of the scanning, enumeration, and brute-forcing modules studied earlier. Using Nmap, Gobuster, and Hydra, I was able to compromise an SSH service, gain user-level access, and retrieve the user flag. Root privilege escalation will be conducted after completing the relevant CEH modules. This session helped bridge the gap between theory and real-world attack simulation.
