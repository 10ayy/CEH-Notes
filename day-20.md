# Day 20 – Hacking Web Servers

## 📚 Module: Web Server Hacking (Module 13)

### 🔍 Topics Covered:

- **What is a Web Server** 
  A web server is software and hardware that uses HTTP and other protocols to respond to client requests made over the World Wide Web.

- **Web Server Security Issues** 
  - Misconfigurations 
  - Default installations 
  - Unpatched vulnerabilities 
  - Directory traversal 
  - Improper file permissions

- **Web Server Operations and Components** 
  - HTTP Daemons (Apache, Nginx, IIS) 
  - Web content (HTML, PHP, ASP.NET) 
  - Scripting engines 
  - Log files and configuration files

- **Types of Web Server Attacks** 
  - Website defacement 
  - Directory traversal attacks 
  - Misconfiguration exploitation 
  - Source code disclosure 
  - Buffer overflow attacks 
  - File upload and inclusion vulnerabilities

- **Web Server Attack Methodology** 
  1. Information gathering 
  2. Scanning and enumeration 
  3. Vulnerability detection 
  4. Gaining access 
  5. Maintaining access 
  6. Clearing tracks

- **Cross Site Scripting (XSS)** 
  - Definition: XSS is a web security vulnerability that allows attackers to inject malicious scripts into websites, compromising the experience of other users. 
  - **Types**:
    - Stored XSS 
    - Reflected XSS 
    - DOM-based XSS 
  - **Prevention Techniques**:
    - Input validation and output encoding 
    - Use of secure frameworks 
    - Proper sanitization of user input
    - Content Security Policy (CSP)

---

## 🧪 Practical Lab:

**Platform Used**: DVWA (Damn Vulnerable Web Application)

### ✅ Activities Performed:
- **File Inclusion Vulnerability**:
  - Explored how improper handling of file paths can lead to sensitive file disclosures or remote code execution.
  
- **File Upload Vulnerability**:
  - Tested how unrestricted file uploads can be abused to upload malicious files or web shells.
  - Learned mitigation techniques such as file type validation, size limitation, and content scanning.

> **Note**: All practicals were executed within a controlled, ethical environment using personal systems and vulnerable machines for educational purposes only.

---

## 📝 Summary:

On **Day 20**, the module on **Web Server Hacking** was initiated. The session covered core concepts including web server operations, attack vectors, and specifically **file inclusion** and **file upload vulnerabilities** using the DVWA platform. XSS types and defense mechanisms were also introduced, strengthening understanding of web-based attacks in real-world scenarios.

---
