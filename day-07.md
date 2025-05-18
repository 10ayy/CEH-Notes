# 📅 Day 07 - CEH v13 Notes
## 📚 Module 4: Enumeration (Continued)

### 🔍 Topics Covered:

- **NetBIOS Enumeration**
  - Basics of NetBIOS over TCP/IP (NBT)
  - Enumerating NetBIOS names using `nbtstat` and Nmap scripts

- **SMB Enumeration**
  - Understanding SMB protocol
  - Tools used:
    - `smbclient`
    - `enum4linux`
    - `smbmap`
  - Enumeration using `msfconsole` modules
    - `auxiliary/scanner/smb/smb_enumusers`
    - `auxiliary/scanner/smb/smb_version`

- **SNMP Enumeration**
  - Basics of SNMP (Simple Network Management Protocol)
  - Using `snmpwalk`, `onesixtyone`, and Metasploit modules
    - `auxiliary/scanner/snmp/snmp_enum`

- **LDAP Enumeration**
  - Lightweight Directory Access Protocol enumeration overview
  - Enumeration using Nmap scripts and Metasploit:
    - `nmap -p 389 --script ldap*`
    - `auxiliary/gather/ldap_search`

- **NTP Enumeration**
  - Basics of NTP (Network Time Protocol) and enumeration of time data
  - Using:
    - `ntptrace`
    - `nmap -sU -p 123 --script=ntp-monlist`

- **SMTP Enumeration**
  - Methods of identifying valid users through VRFY, EXPN commands
  - Using `telnet`, `nmap`, and Metasploit:
    - `auxiliary/scanner/smtp/smtp_enum`

---

### 🧪 Hands-on Practicals

- Enumerated SMB shares using Metasploit and Nmap
- Brute-forced user accounts using `enum4linux`
- Identified active SNMP services and extracted data
- Gathered domain and user data from LDAP with Metasploit modules
- Enumerated SMTP services to identify users using Metasploit scripts

---

### 🧠 Key Takeaways

- Enumeration is **active information gathering** and often yields **critical usernames, shares, and protocols**.
- Different protocols require specialized tools/scripts for efficient data extraction.
- Strong enumeration increases the **probability of successful exploitation** in later phases.

---

> 🛠️ *Tools practiced: `nbtstat`, `enum4linux`, `smbclient`, `msfconsole`, `snmpwalk`, `ntptrace`, `telnet`, Nmap scripts.*

---

### 📌 Summary

Day 07 focused on deepening the enumeration process by exploring protocols such as NetBIOS, SMB, SNMP, LDAP, NTP, and SMTP. Practical exposure to enumeration through tools like msfconsole strengthened understanding of how to extract sensitive information from network services—laying the groundwork for vulnerability analysis and eventual exploitation.
