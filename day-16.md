# Day 16 – DoS Tools (Practical) & Introduction to Session Hijacking (Module 11)

## 🛠️ Practical: Social Engineering & DoS Tools (Continued)

The day began with hands-on practice using **DoS tools and traffic analysis** to understand how flooding and packet manipulation can be carried out, and how they are interpreted at the packet level using traffic monitoring tools like **Wireshark**.

### ⚙️ Tools Practiced:

1. **hping3**
   - Used to generate custom TCP/IP packets.
   - Command: `hping3 -S <target-ip> -p 80 --flood`
   
2. **ping flooding**
   - Command: `ping <target-ip> -s 1000 -f`
   - Sends fragmented ICMP packets to overload the buffer capacity.

3. **GoldenEye**
   - A stress-testing tool to simulate HTTP-based DoS.
   - Tool used to flood the web server with HTTP GET/POST requests.

4. **Metasploit (msfconsole)**
   - Used to launch a simulated DoS attack and monitor the payload’s behavior.

### 🔍 Traffic Monitoring:
- **Wireshark** was used to observe network traffic during DoS attacks.
- Tracked SYN floods, large ICMP requests, and HTTP request floods.
- Real-time analysis of request/response behavior under DoS conditions.

> ⚠️ **Disclaimer**: All practices were executed in a controlled lab environment using test systems only. No real systems were targeted or harmed.

---

## 📚 Introduction to Module 11 – Session Hijacking

After the tool-based exercises, a new theoretical module was initiated focusing on **Session Hijacking**, one of the most critical and often underestimated security risks in web applications.

---

## 📖 Concepts Covered:

### 🔹 What is a Session?
- A **session** is a semi-permanent interactive information interchange between two or more communicating devices.
- Maintained through **Session IDs**, often stored in **cookies**, URL, or hidden form fields.

### 🔹 What is Session Hijacking?
- Unauthorized exploitation of a valid computer session to gain unauthorized access.
- The attacker takes over a session between two computers.

---

## 🧠 Why Session Hijacking Works:
- Poor session ID management.
- Insecure transmission of session tokens.
- Lack of encryption (HTTP instead of HTTPS).
- Vulnerable or exposed cookies.

---

## 🔄 Types of Session Hijacking:

| Type | Description |
|------|-------------|
| **Active Hijacking** | Attacker takes over an ongoing session - Application level hijacking |
| **Passive Hijacking** | Attacker monitors session without disrupting it - Network level hijacking |

---

## 🧪 Methods to Obtain Session IDs:

1. **Session Prediction** – Guessing predictable session tokens.
2. **MITM (Man-in-the-Middle)** – Intercepting the session via network sniffing.
3. **MITB (Man-in-the-Browser)** – Trojan intercepting session data inside the browser.
4. **Sniffing (Wireshark, tcpdump)** – Capturing data packets containing session IDs.
5. **Malware Attack** – Keyloggers or backdoors that extract session tokens.
6. **Cross-Site Scripting (XSS)** – Stealing session ID via injected scripts.
7. **Proxy Servers** – Capturing session data through insecure proxies.

---

## 📝 Summary

Day 16 began with the execution of advanced DoS tools such as **hping3**, **GoldenEye**, and **Metasploit** payloads, while monitoring the attack impact using **Wireshark**. Later, I initiated **Module 11 – Session Hijacking**, where I developed a foundational understanding of session mechanics, the vulnerabilities in session management, and various attack vectors used to hijack session data from clients and servers.

---
