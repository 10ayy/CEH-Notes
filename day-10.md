# Day 10 – System Hacking & Authentication

## 📘 Module: System Hcking (Module 6)

On Day 10, the focus was on **System Hacking**, a critical area that demonstrates how systems—particularly Windows and Linux—can be compromised even when not connected to a network. The session also covered fundamental authentication mechanisms used in enterprise environments.

---

## 📚 Topics Covered
- Windows Authentication Mechanisms
- Security Account Manager (SAM) File
- Windows Domain Controller
- Windows Offline Password Reset (Ethical Note)
- Linux Offline System Compromise

---

## 🔒 Windows Authentication Mechanisms

- **Windows Management Security**:
  - **LM Hash (LAN Manager Hash)**:
    - Outdated and highly insecure.
    - Uses DES encryption and is vulnerable to brute force attacks.
  - **NTLM Hash (New Technology LAN Manager)**:
    - Improved over LM hash but still vulnerable to pass-the-hash attacks.
  - **Kerberos Authentication**:
    - Secure ticket-based protocol used in domain environments.
    - Works on the basis of symmetric key cryptography and time-based tokens.

---

## 📁 Security Account Manager (SAM) File

- The **SAM file** stores hashed versions of user passwords in Windows.
- Located at: `C:\Windows\System32\Config\SAM`
- Can only be accessed if Windows is offline or compromised via privilege escalation.

---

## 🏢 Windows Domain Controller

- A **Domain Controller (DC)** is a server that responds to authentication requests within a Windows domain.
- Handles:
  - User logins
  - Group policy enforcement
  - Kerberos ticketing
- Compromising a DC allows **complete domain control**, often the final goal of attackers in enterprise breaches.

---

## 💻 Windows Offline Password Reset (Ethical Note)

- Demonstration (theoretical only) of **bypassing Windows local account password** by:
  - Booting with a customized **ISO image**.
  - Triggering a system error to access administrative tools.
> **⚠️ Note**: The actual procedure is **not uploaded or shared** due to **ethical and responsible disclosure guidelines**.

---

## 🐧 Linux Offline System Compromise

- Method to change root or user password in Linux-based distros (e.g., Kali, Ubuntu) by:
  - Booting into **single-user mode** or
  - Using a **live CD** and mounting the file system or
  - Updating the **GRUB menu**.
> **⚠️ Note**: The actual procedure is **not uploaded or shared** due to **ethical and responsible disclosure guidelines**.

- This demonstrates how physical access equals root access, underscoring the importance of full disk encryption.

---

## 📝 Summary

On Day 10, a comprehensive overview of offline system hacking was explored, including Windows authentication models like LM, NTLM, and Kerberos. Important system components such as the SAM file and Domain Controllers were discussed. The session also introduced techniques to reset or modify system passwords on both Windows and Linux, reinforcing the importance of physical security and encryption to protect systems from offline threats.
> *Onlne system hacking can also be done with the help of msfvenom or getting the reverse shell/remote connectio of the system*
