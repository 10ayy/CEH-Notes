# Day 28 – Practical Session: Hacking Wi-Fi Networks

## 📶 Session Overview:
On Day 28, a **hands-on lab session** was conducted to deepen our understanding of **wireless network exploitation techniques**, specifically focusing on **capturing Wi-Fi handshakes**, analyzing traffic, and simulating real-world wireless attacks in a controlled ethical environment.

---

## 🔧 Topics Practically Covered

### 🎯 1. Capturing Wi-Fi Handshake
- **Objective**: Capture the 4-way WPA/WPA2 handshake between a wireless client and the access point.
- **Tool Used**: `airmon-ng`, `airodump-ng`, `aireplay-ng`, `aircrack-ng`
- Handshake files saved for offline password cracking.

### 📡 2. What is Monitor Mode?
- Monitor mode allows a wireless network interface card (NIC) to **listen to all wireless traffic** within range, even if it is not intended for the NIC.
- Enabled via:
  ```bash
  airmon-ng start wlan0
  ```
### 💻 3. Why Wi-Fi Adapters are Required
- External USB Wi-Fi adapters (with monitor mode support) are used because most internal laptop Wi-Fi cards do not support packet injection or monitoring.
- Recommended chipsets: Atheros, Realtek RTL8812AU, MediaTek Ralink

### 🔓 4. Cracking the Wi-Fi Password
- Captured handshake file is used with a wordlist (e.g., rockyou.txt) to brute-force the password:
   ```bash
    aircrack-ng capturefile.cap -w rockyou.txt
   ```

### 🚫 5. Deauthentication (Deauth) Attack
- Forcing a device to disconnect from a network to capture a fresh handshake.
```bash
    aireplay-ng --deauth 10 -a <BSSID> wlan0mon
```

### 🎭 6. Evil Twin Attack
- Creation of a fake access point (rogue AP) with the same SSID as the target to lure users.
- Tools: `airbase-ng`, `hostapd`, or custom scripts like `Fluxion`

> *📌 All attacks were executed in a sandboxed, ethical lab setup against personal or test routers under direct guidance and for academic purposes only.*

---

## 🎓 Training Milestone Achieved

- I am pleased to share that I have successfully completed the CEH (Certified Ethical Hacker) training from Craw Security. Over the past weeks, I have documented each module and practical session thoroughly.
- Moving forward:
    - I will now shift my focus to preparing for the **official EC-Council CEH v12 examination**.
    - My preparation strategy includes:
        - Reviewing **EC-Council official PDFs**
        - Practicing **hands-on labs and scenarios**
        - Strengthening both **theoretical knowledge** and **practical skillsets**

*I may continue to share future progress, resources, or notes derived from the official EC-Council materials, subject to permissible use.*

---

## 📝 Summary:

On **Day 28**, a complete practical session on **Wi-Fi hacking techniques** was conducted. I learned to **capture and crack WPA handshakes**, understand **monitor mode**, and simulate **deauth and Evil Twin attacks** using industry-standard tools. With this, my formal training phase with Craw Security concludes, and I now step into **certification-focused self-study** with renewed confidence.
