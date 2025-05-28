# Day 13 – Sniffing (Module 8)

## 🧪 Sniffing Attacks and Network Reconnaissance

On Day 13, I began working on **Module 8: Sniffing** in the CEH curriculum. This module introduced key concepts in **network surveillance and attack tactics** targeting **Layer 2 (Data Link Layer)**, focusing on sniffing techniques, network components, and corresponding exploitation tools.

---

## 🌐 Networking Fundamentals Refresher

### 🔌 Key Components:
- **Router** – Connects different networks (Layer 3 device)
- **Switch** – Connects devices within the same LAN (Layer 2 device)
- **LAN (Local Area Network)** – Private network covering a limited area such as a home, school, or office

---

## 🕵️ What is Sniffing?

Sniffing is the process of monitoring and capturing all data packets passing through a given network using sniffing tools. It is often the **first step in a man-in-the-middle (MITM)** or passive reconnaissance attack.

---

## 🧠 Key Concepts Covered:

### 🆔 MAC Address:
- Media Access Control (MAC) address is a hardware identifier for a network interface.

### 📋 CAM Table:
- Content Addressable Memory (CAM) Table is maintained by switches to map MAC addresses to specific physical ports.
- Attackers often exploit this by **flooding or poisoning** the table to perform sniffing attacks.

---

## ⚠️ Types of Sniffing Attacks:

| Attack Type         | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| **ARP Poisoning**   | Sends spoofed ARP messages to associate the attacker's MAC with the IP of another host |
| **MAC Spoofing**    | Changes the attacker's MAC to impersonate another device                    |
| **MAC Flooding**    | Overloads the CAM table causing the switch to behave like a hub (broadcast) |
| **DHCP Starvation** | Exhausts the DHCP IP address pool by sending multiple fake requests         |

---

## 🛠️ Tools and Techniques

### 🔥 ARP Poisoning:
- `ettercap` – Used for man-in-the-middle ARP spoofing attacks.
- `bettercap` – Advanced, modular MITM attack tool with real-time monitoring.

```bash
# Sample Bettercap usage
sudo bettercap -iface eth0
```

### 🎭 MAC Spoofing:
- `macchanger` – Change MAC address in Kali Linux.
- `macof` – Tool to flood the CAM table.
- `Technitium MAC Address Changer` – Windows utility for MAC spoofing.

```bash
# MAC address spoofing using macchanger
sudo macchanger -r eth0
```

### 🌩️ DHCP Starvation:
- `yersinia` – Powerful Layer 2 attack tool.

```bash
# Launching yersinia GUI mode
sudo yersinia -G
```

---

## 📝 Summary

Day 13 focused on understanding how sniffing attacks exploit Layer 2 protocols and how these can be executed using specialized tools. I reviewed essential networking components, dissected multiple sniffing attack types, and practiced with ettercap, bettercap, macchanger, macof, yersinia, and Technitium. These tools and concepts are foundational for advanced network-based MITM attacks, packet capturing, and traffic manipulation techniques.
