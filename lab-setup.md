# 🧪 CEH Lab Setup for Practical Exercises

This guide outlines how to set up a local virtual lab environment to practice practical modules of the **Certified Ethical Hacker (CEH v13)** course.

The lab includes:
- **Attacker Machine**: Kali Linux or Parrot OS
- **Victim Machines**: Metasploitable 2 and Windows 10
- **Platform**: VMware Workstation or VirtualBox (Cross-compatible)

> This setup ensures a secure, isolated environment to test footprinting, scanning, enumeration, vulnerability analysis, and exploitation techniques.

## 🛠️ Tools Required

| Tool                | Purpose                        |
|---------------------|--------------------------------|
| VMware Workstation  | Virtualization Platform        | 
| VirtualBox (alt)    | Free virtualization (optional) | 
| Kali Linux ISO      | Attacker OS                    | 
| Parrot OS ISO (alt) | Attacker OS (privacy-focused)  | 
| Metasploitable 2    | Vulnerable Linux OS            | 
| Windows 10 ISO      | Vulnerable OS for Pentesting   | 

## 🧱 Network Configuration

- Use Host-Only or Internal Network mode for isolation (recommended).
- All machines must be on the same virtual subnet for connectivity.

| Machine         | IP Example     | Role           |
|-----------------|---------------------------------|
| Kali Linux      | 192.168.100.10 | Attacker       | 
| Metasploitable2 | 192.168.100.20 | Victim Linux   | 
| Windows 10      | 192.168.100.30 | Victim Windows |

> Avoid NAT or Bridged during exploitation to stay off public networks.

## ⚙️ Step-by-Step Setup Procedure
### 🖥️ Step 1: Install VMware Workstation (or VirtualBox)

- Download and install from the official site.
- Reboot if prompted.

### 🐉 Step 2: Set Up Kali Linux or Parrot OS (Attacker)

- Create a new VM → Select ISO → Kali or Parrot ISO
- Set:
    - CPU: 2 Cores
    - RAM: 4GB (minimum)
    - Disk: 30GB+
    - Network: Host-Only or Internal Network
- Complete OS installation.
- Update the OS and tools:

```bash
    sudo apt update && sudo apt upgrade -y
```

### ☠️ Step 3: Set Up Metasploitable 2 (Linux Victim)

- Import ```.vmx``` file or open ```.ova``` in VMware.
- Configure:
    - RAM: 1GB
    - Network: Same ```Host-Only``` or ```Internal```
- Boot and **do not update** — vulnerabilities must remain intact.

### 🪟 Step 4: Set Up Windows 10 (Victim Machine)

- Create VM → Load Windows 10 ISO.
- Install OS normally.
- Install:
    - Vulnerable applications (e.g., outdated browsers, FTP servers, etc.)
- Disable firewall/defender (for CEH testing only):

```powershell
    Set-NetFirewallProfile -Profile Domain,Public,Private -Enabled False
```

- Add user accounts for enumeration/brute-force practice.

### 🌐 Step 5: Test Network Connectivity

From Kali or Parrot:

```bash
ping 192.168.100.20   # Metasploitable
ping 192.168.100.30   # Windows 10
```

If unreachable, ensure:

- All VMs are powered on
- All are on same Host-Only/IntNet
- Firewalls are off (esp. on Windows)

### 📂 Step 6: Snapshot the Clean State

Before starting exercises, take a VM snapshot of each system for easy rollback after exploitation.

## 📌 Summary

This virtual lab setup enables a safe and controlled environment to simulate real-world attack scenarios and apply CEH tools and techniques. It serves as a foundational workspace for mastering ethical hacking modules while ensuring no exposure to external networks or live systems.
