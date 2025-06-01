# Day 15 – Social Engineering Tools (Practical) & Introduction to DoS (Module 10)

## 🛠️ Recap: Social Engineering Practical (Module 9)

On Day 15, I continued with the **Social Engineering module** by performing hands-on practice using three key tools in a controlled lab environment. These tools simulate real-world social engineering attacks and provide red teamers with insight into phishing techniques and social deception vectors.

### ⚙️ Tools Practiced:
- **Zphisher**: Used for deploying phishing pages for platforms like Instagram, Facebook, and others.
- **CamPhish**: Utilized to simulate webcam access and geolocation phishing.
- **SEToolkit**: Created fake login pages and executed social engineering attack vectors like spear phishing.

> ⚠️ **Note**: Due to ethical and legal considerations, practical demonstrations and sensitive screenshots are not included in this public repository. These tools were executed in isolated lab environments with no real-world targeting.

---

## 📚 Introduction to Module 10 – Denial of Service (DoS)

The second half marked the start of **Module 10: Denial of Service (DoS)**, where I explored how attackers can render systems and services unavailable by overwhelming them with traffic or requests.

---

## 📖 Concepts Covered:

### 🔹 What is DoS and DDoS?
- **DoS (Denial of Service):** An attack where a single system sends a large volume of traffic to crash or slow down a service.
- **DDoS (Distributed Denial of Service):** Similar to DoS but performed by **multiple systems (botnets)** simultaneously, increasing attack volume and scale.

---

## 🤖 Related Terminologies:

| Term | Description |
|------|-------------|
| **Botnet** | A network of compromised systems ("zombies") controlled by an attacker |
| **Peer-to-Peer (P2P) Connection** | Distributed control system used to manage large botnets |

---

## 🧨 DoS/DDoS Attack Techniques:

1. **Bandwidth Attacks** – Saturating the bandwidth capacity
2. **Service Request Floods** – Sending massive amounts of legitimate-looking requests to exhaust server resources
3. **SYN Attack** – Exploiting TCP three-way handshake to exhaust server resources
4. **SYN Flooding** – Repeated SYN requests without final ACK
5. **ICMP Flood** – Ping requests to overload target (Ping Flood, Ping of Death)
6. **Botnet-Based DDoS** – Coordinated request storm from globally infected devices

---

## 💥 Types of DoS/DDoS Attacks:

- **Ping of Death Attack:** Malicious oversized ping packets crashing the system
- **Smurf Attack:** Spoofed ICMP packets sent to a network's broadcast address, overwhelming the victim

---

## 🛡️ DoS/DDoS Prevention Measures:

- Implement **firewalls and rate limiting**
- Use **anti-DDoS services (e.g., Cloudflare, AWS Shield)**
- **Network monitoring** and early anomaly detection
- **System hardening** and patching vulnerabilities

---

## 🧭 Basic Categories of DoS/DDoS Attacks:

| Category | Description |
|----------|-------------|
| **Volume-Based Attacks** | Flood the bandwidth |
| **Protocol Attacks** | Target server resources |
| **Application Layer Attacks** | Exploit vulnerabilities in web servers/applications |

---

## ✅ Summary

Day 15 consisted of completing hands-on practice using popular social engineering tools, reinforcing my understanding of phishing attack vectors. In the second half, I was introduced to the **Denial of Service** module, gaining clarity on how DoS and DDoS attacks function at various layers, their methodologies, and the infrastructure behind large-scale internet disruptions.
