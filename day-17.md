# Day 17 – Session Hijacking Practical & Introduction to Web Application Hacking (Module 14)

## 🧪 Practical: Session Hijacking (Continued)

The day began with the **hands-on practical** for session hijacking using **Burp Suite Community Edition**.

### ⚙️ Tools & Techniques:

- **Burp Suite Community Edition** was utilized to intercept and manipulate HTTP requests.
- The target platform used for the lab was **TestPHP.vulnweb.com**, a vulnerable test site for ethical hacking practice.
- The **goal** was to identify and capture the session token/cookie of a user and hijack the session by replicating the session environment in another browser.

> ⚠️ **Ethical Note**: The demonstration was conducted in a lab environment using a public test site. Due to ethical considerations and platform usage guidelines, the detailed steps, screenshots, and session credentials are not included in this document.

---

## 📚 Introduction to Module 14 – Hacking Web Applications

After completing the practicals, a new theoretical module was introduced: **Web Application Hacking**.

---

## 🧠 Key Concepts Covered:

### 🔹 What is a Web Application?
- A **web application** is a client-server software application that runs on a web browser.
- Accessible via a browser through the internet or intranet.

### 🔹 How Web Applications Work:
1. **Client Side (Frontend)** – User interface that interacts with the user.
2. **Server Side (Backend)** – Logic, database handling, and data processing.

### 💻 Technologies:
- **Frontend Languages**: HTML, CSS, JavaScript
- **Backend Languages**: PHP, Python, Java, Ruby, Node.js, etc.

---

## 🧾 Important Terms:

| Term | Description |
|------|-------------|
| **Web Server** | Software that handles HTTP requests (e.g., Apache, Nginx) |
| **Server Administrator** | Manages server operations and configurations |
| **Application Administrator** | Manages deployment and maintenance of web apps |
| **Client** | The end user accessing the web app through a browser |

---

## 🔐 OWASP Top 10 Introduction:

The **OWASP Top 10** is a standard awareness document for developers and web application security. It represents a broad consensus about the most critical security risks to web applications.

### Common Categories (Discussed Briefly):
- A01: Broken Access Control
- A02: Cryptographic Failures
- A03: Injection
- A04: Insecure Design
- A05: Security Misconfiguration
- A06: Vulnerable and Outdated Components
- A07: Identification and Authentication Failures
- A08: Software and Data Integrity Failures
- A09: Security Logging and Monitoring Failures
- A10: Server-Side Request Forgery (SSRF)

---

## 📝 Summary

On Day 17, the **practical implementation of session hijacking** was conducted using **Burp Suite CE**, helping me understand how HTTP cookies and session tokens can be exploited in insecure web applications. After the lab, I started **Module 14 – Web Application Hacking**, which laid the foundation for understanding how web applications function, the architecture of client-server interaction, and introduced the **OWASP Top 10**, a vital guideline for identifying and mitigating web application vulnerabilities.

---
