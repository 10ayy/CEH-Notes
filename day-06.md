# 📅 Day 06 – Module 4: Enumeration

## 📘 Topics Covered
- What is Enumeration?
- Enumeration Techniques
- FTP Enumeration via Nmap
- Telnet and SSH Enumeration
- SSH Brute Force via Nmap Script
- Gaining Access with msfconsole (Metasploit)

---

## 🔍 What is Enumeration?

Enumeration is the **process of extracting user names, machine names, network resources, shares, and services** from a system. It is an active process that builds on the scanning phase and reveals detailed information about the target system.

> 🎯 Enumeration is essential for identifying potential entry points and preparing for exploitation.

---

## 🧰 Enumeration Techniques

- **FTP Enumeration**
- **Telnet Enumeration**
- **SSH Enumeration**
- **SNMP, SMB, LDAP** (covered later)

Each service provides a different scope of information and is explored using specialized tools or scripts.

---

## 📂 FTP Enumeration via Nmap

### 🔧 Command Example:

```bash
nmap -p 21 --script ftp-anon,ftp-bounce,ftp-syst <target-ip>
```

### ✅ Objectives:

- Check for anonymous login
- Determine FTP server type
- Explore directory listings and banners 

--- 


## 🧑‍💻 Telnet Enumeration

Telnet, although outdated and insecure, still exists in legacy systems.

- Use Telnet client to manually connect and identify login prompts
- Observe service banners, credentials, or default settings

```bash
telnet <target-ip> 23
```

## 🔐 SSH Enumeration via Nmap

### 🔍 Nmap Commands:

```bash
nmap -p 22 --script ssh-auth-methods,ssh-hostkey,ssh-brute <target-ip>
```
- ssh-auth-methods: Shows supported authentication methods
- ssh-brute: Attempts brute-forcing with default or given user/pass
- ssh-hostkey: Extracts host public key

## 💥 SSH Brute Forcing (Nmap + Metasploit)
### 🔓 Brute Force Using Nmap

```bash
nmap -p 22 --script ssh-brute --script-args userdb=users.txt,passdb=pass.txt <target-ip>
```

### 🛠️ Using Metasploit (msfconsole)

```bash
use auxiliary/scanner/ssh/ssh_login
set RHOSTS <target-ip>
set USERNAME <username>
set PASSWORD <password>
run
```

> *✅ Successfully gained access to msfadmin user on target via brute force and validated it in practice.*

## 🧪 Practical Highlight

Performed hands-on exercises to:

- Use nmap scripts to enumerate SSH credentials
- Gain shell access via msfconsole
- Observe how enumeration leads to actual system access when weak credentials exist

## 📌 Summary
- Enumeration provides critical details beyond what scanning reveals
- FTP, Telnet, and SSH can leak sensitive service-level information
- Automation via Nmap scripts and Metasploit modules improves effectiveness
- Real-world exercise: Successfully brute-forced and accessed an SSH service

> 🔐 Takeaway: Enumeration is where ethical hackers transform reconnaissance into actionable intelligence. Mastery here leads directly into the exploitation phase.
