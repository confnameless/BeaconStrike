<div align="center">

# 📡 BEACONSTRIKE
**The Ultimate WPA3/WPA2 Channel Switch Exploit Toolkit**

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Linux-lightgrey?style=for-the-badge&logo=linux&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg?style=for-the-badge)

<br>

<a href="#-features">Features</a> •
<a href="#-installation">Installation</a> •
<a href="#-usage">Usage</a> •
<a href="#-legal-disclaimer">Disclaimer</a>

</div>

---

## 💀 What is BeaconStrike?

**BeaconStrike** is a next-generation wireless auditing tool designed to challenge **WPA3 Security**.

While traditional deauthentication attacks are rendered useless by WPA3's **Protected Management Frames (PMF)**, BeaconStrike bypasses these protections by exploiting the **Channel Switch Announcement (CSA)** mechanism found in 802.11 beacons. It surgically injects spoofed management frames (IE 37) to force connected clients onto "dead" channels, effectively disconnecting them without triggering standard intrusion detection systems.

## 🔥 Features

| Feature | Description |
| :--- | :--- |
| **🛡️ PEP-668 Bypass** | Automatically creates a hidden Virtual Environment (`.venv`) to bypass "Externally Managed Environment" errors on Kali 2024 & Ubuntu. |
| **📦 Auto-Dependency** | Detects your OS (Debian/Arch/Fedora) and auto-installs system tools (`aircrack-ng`) and Python libraries. |
| **👁️ God Mode Scanner** | Live, auto-updating dashboard of APs and Clients with signal strength (RSSI) sorting. |
| **🎯 Laser Targeting** | Select a specific client MAC address to kick, or broadcast to the entire network. |
| **🔄 Self-Healing** | Built-in updater checks GitHub for the latest patches and installs them automatically. |

---

## 📥 Installation

BeaconStrike is designed to be "Download & Run." It works out-of-the-box on **Kali Linux**, **Parrot OS**, **Arch Linux**, and **Ubuntu**.

### 1. Clone the Repository
```bash
git clone [https://github.com/confnameless/BeaconStrike.git](https://github.com/confnameless/BeaconStrike.git)
cd BeaconStrike

2. Make Executable
Bash

chmod +x beaconstrike.py
3. Run (Root Required)
Bash

sudo ./beaconstrike.py
Note: You do NOT need to manually install pip requirements. The script's bootstrapper handles all library installations on the first launch.

🚀 Usage Guide
Launch the Tool: Run with sudo. The script will automatically kill interfering processes (NetworkManager).

Select Interface: Choose your wireless card. Monitor mode is enabled automatically.

Scan Targets: A live table will appear. Press Ctrl+C to stop scanning and select a target AP.

Attack: Choose a specific victim client or "Broadcast" to kick everyone.

Results: Watch as the target device disconnects or struggles to maintain a connection.

📸 Interface
Plaintext

██████╗ ███████╗ █████╗  ██████╗ ██████╗ ███╗   ██╗
██╔══██╗██╔════╝██╔══██╗██╔════╝██╔═══██╗████╗  ██║
██████╔╝█████╗  ███████║██║     ██║   ██║██╔██╗ ██║
██╔══██╗██╔══╝  ██╔══██║██║     ██║   ██║██║╚██╗██║
██████╔╝███████╗██║  ██║╚██████╗╚██████╔╝██║ ╚████║
╚═════╝ ╚══════╝╚═╝  ╚═╝ ╚═════╝ ╚═════╝ ╚═╝  ╚═══╝
            [ MADE BY CONFNAMELESS ]
(Place a screenshot of your tool running here. Example: ![Screenshot](assets/demo.png))

⚠️ Legal Disclaimer
[!WARNING] FOR EDUCATIONAL PURPOSES ONLY.

The use of this script is intended for authorized penetration testing and security research only.

Do not use this tool on networks you do not own or have explicit permission to test.

The author (Confnameless) is not responsible for any misuse or damage caused by this program.

Unlawful interception of wireless communications is a crime in most jurisdictions.

👤 Credits
Author: Confnameless

Core Logic: Scapy

UI Framework: Rich
