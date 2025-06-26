# Day 26a – Module 17: Hacking Mobile Platforms

## 📱 What is Mobile Hacking?
Mobile hacking refers to **exploiting vulnerabilities in mobile devices** such as smartphones and tablets, or the mobile applications and operating systems they run. The goal is typically to gain unauthorized access, control, or extract sensitive information.

---

## 🔒 OWASP Top 10 Mobile Risks
These are the most critical mobile security risks identified by OWASP:

1. Improper Platform Usage  
2. Insecure Data Storage  
3. Insecure Communication  
4. Insecure Authentication  
5. Insufficient Cryptography  
6. Insecure Authorization  
7. Client Code Quality Issues  
8. Code Tampering  
9. Reverse Engineering  
10. Extraneous Functionality

---

## 🦠 What is Mobile Malware?
Mobile malware is malicious software specifically designed to **target mobile devices**. It can steal data, spy on users, or take control of device functionality.

---

## 🎯 What is an Attack Vector?
An attack vector is a **path or means** by which a hacker gains access to a mobile device or network in order to deliver a malicious payload or achieve unauthorized access.

---

## 🤖 What is Android RAT?
An **Android RAT (Remote Access Trojan)** is a type of malware that allows an attacker to **remotely control a victim’s Android device**, including:
- Accessing files
- Recording audio or video
- Capturing keystrokes
- Reading messages or call logs

---

## 🧬 Types of Android RATs:
- **Open-Source**:
  - AhMyth
  - L3MON
  - AndroRAT
- **Paid/Commercial**:
  - DroidJack
  - SpyNote
  - NexSpy

---

## 🌐 Scope of Android RAT:
- Espionage and surveillance
- Blackmail or extortion
- Data exfiltration (contacts, messages, passwords)
- Remote shell execution
- Device manipulation (camera, mic, GPS)

---

## 🧰 Tools Used in Android RAT Deployment:
### GUI-Based RAT Tools:
- **AhMyth** – Electron-based open-source Android RAT with a graphical interface
- **L3MON** – Web-based Android RAT management platform

### CLI-Based (Metasploit Integration):
- **msfvenom** – Used to generate malicious APK payloads
- **msfconsole** – Used to handle reverse TCP connections from infected Android devices

---

## 🧪 Practical Exercises:
- Created Android RAT payloads using:
  - `AhMyth`
  - `msfvenom` → `android/meterpreter/reverse_tcp`
- Delivered APKs to the target device via HTTP server
- Accessed victim session through `msfconsole`

📌 **Note**: Practical demonstrations were performed in a controlled lab environment for educational purposes and are **not uploaded to GitHub** due to ethical and legal restrictions.

---

## 📝 Summary:

On **Day 26**, Module 17 on **Hacking Mobile Platforms** was completed. The session covered **OWASP Top 10 Mobile Risks**, **Android RATs**, malware deployment techniques, and hands-on labs using **AhMyth** and **msfvenom**. The importance of ethical boundaries and responsible disclosure was emphasized when dealing with mobile exploitation and RAT operations.

---
