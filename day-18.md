# Day 18 – Practical: Web Application Hacking (DVWA)

## 🧪 Practical Lab: Web Application Hacking Using DVWA

The focus of today's session was the **hands-on practical implementation** of web application attacks using the **Damn Vulnerable Web Application (DVWA)**.

---

## 🧰 Tools & Environment:

- **DVWA** (Damn Vulnerable Web Application)  
  - Target machine: DVWA hosted on **Metasploitable 2** (or can be installed locally on Kali using `sudo apt install dvwa`)
- **Burp Suite Community Edition** – used as the proxy to inspect and manipulate HTTP requests.
- **Mozilla Firefox** – configured to route traffic through Burp Suite.

---

## ⚙️ Lab Setup Notes:

- If running DVWA on **Metasploitable 2**: access the DVWA in browser via `http://<Metasploitable-IP>/dvwa`.
- If using DVWA locally on Kali:
  ```bash
  dvwa-start
  ```
- Access it at: http://127.0.0.1:42001/login.php
- Firefox Proxy Configuration:
    - Manual proxy setup → HTTP Proxy: 127.0.0.1, Port: 8080
    - Ensure “Use this proxy server for all protocols” is selected.
- In Burp Suite:
    - Proxy → Intercept → ON
    - Analyze and manipulate HTTP requests sent to DVWA.

---

## 🔍 Attack Vectors Practiced:

🔸 **1. Brute Force Attack**
- Module: Brute Force (Login)
- Goal: Attempt username/password combinations to gain access.
- Observed how HTTP POST requests can be intercepted and repeated with modified credentials using Burp Repeater.

🔸 **2. Command Execution**
- Module: Command Injection
- Objective: Inject OS commands into vulnerable fields and analyze the results.
- Successfully injected commands like ; `ping` to enumerate the system.

🔸 **3. Cross-Site Request Forgery (CSRF)**
- Module: CSRF
- Performed unauthorized actions on behalf of a user by crafting malicious requests and sometines changing the user credentials.
- Studied how session tokens are crucial in preventing CSRF attacks.

> ⚠️ **Note**: Due to ethical and legal considerations, practical demonstrations and sensitive screenshots are not included in this public repository.

---

## 🧠 Key Learnings:

- DVWA is a powerful testbed for practicing various OWASP Top 10 vulnerabilities.
- Burp Suite is essential for traffic manipulation, session analysis, and attack simulation.
- Realized the importance of session tokens, input validation, and secure coding practices in mitigating these attacks.

---

## 📝 Summary:

On Day 18, I executed a series of practical attacks on DVWA, including brute force, command injection, and CSRF. The practical demonstrated how vulnerable web applications can be exploited using tools like Burp Suite and highlighted the importance of proper input handling, session security, and secure web architecture. This session provided a comprehensive understanding of how real-world web application attacks are executed and detected.
