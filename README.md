# BeaconStrike
The ultimate WPA3 channel-switch exploit tool. Bypass PMF protections and force client disconnects with automated CSA injection. Works on Kali, Arch, and Ubuntu.
____________________________________________________________________________________________________________________________________________________________________

# 📡 BeaconStrike

> **The Ultimate WPA3/WPA2 Channel Switch Exploit Toolkit**
> *Seamlessly audit wireless networks by forcing client disconnections via CSA injection.*

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Platform](https://img.shields.io/badge/Platform-Linux%20(Kali%2FArch%2FDebian)-lightgrey)
![License](https://img.shields.io/badge/License-MIT-green)
![MadeBy](https://img.shields.io/badge/Made%20By-CONFNAMELESS-red)

---

## 💀 What is BeaconStrike?

**BeaconStrike** is an advanced, automated Python 3 script designed to test the resilience of Wi-Fi clients against **Channel Switch Announcement (CSA)** attacks.

Unlike traditional deauthentication attacks that are blocked by WPA3's **Protected Management Frames (PMF)**, BeaconStrike exploits the roaming logic in modern devices. It injects spoofed Beacon frames containing **IE 37 (Channel Switch Announcement)**, tricking connected clients into jumping to a "dead" channel (e.g., Channel 140), effectively disconnecting them without triggering intrusion detection systems.

### 🔥 Key Features

* **🛡️ PEP-668 Bypass:** Automatically creates a hidden Virtual Environment (`.venv`) to fix "Externally Managed Environment" errors on modern Linux distros (Kali 2024, Ubuntu 24.04).
* **📦 Auto-Dependency Magic:** Detects your OS (Debian/Arch/Fedora) and automatically installs system tools (`aircrack-ng`) and Python libraries (`Scapy`, `Rich`).
* **👁️ God Mode Scanner:** Live, auto-updating table of all nearby APs and connected Clients with signal strength (RSSI) sorting.
* **🎯 Precision Targeting:** surgically target a single client MAC or nuke the entire network (Broadcast).
* **🔄 Self-Updating:** Built-in engine checks GitHub for updates and patches itself automatically.

---

## 📥 Installation

BeaconStrike works out of the box on almost any Linux system (Kali, Parrot, Ubuntu, Arch).

```bash
# 1. Download the script
wget [https://raw.githubusercontent.com/confnameless/BeaconStrike/main/beaconstrike.py](https://raw.githubusercontent.com/confnameless/BeaconStrike/main/beaconstrike.py)

# 2. Make it executable
chmod +x beaconstrike.py

# 3. Run it (Root is required for hardware access)
sudo ./beaconstrike.py

Note: You do not need to install pip libraries manually. The script will handle everything on the first run.

📸 Screenshots
Plaintext

██████╗ ███████╗ █████╗  ██████╗ ██████╗ ███╗   ██╗
██╔══██╗██╔════╝██╔══██╗██╔════╝██╔═══██╗████╗  ██║
██████╔╝█████╗  ███████║██║     ██║   ██║██╔██╗ ██║
██╔══██╗██╔══╝  ██╔══██║██║     ██║   ██║██║╚██╗██║
██████╔╝███████╗██║  ██║╚██████╗╚██████╔╝██║ ╚████║
╚═════╝ ╚══════╝╚═╝  ╚═╝ ╚═════╝ ╚═════╝ ╚═╝  ╚═══╝
            [ MADE BY CONFNAMELESS ]
⚠️ Legal Disclaimer
FOR EDUCATIONAL PURPOSES ONLY.

The use of this script is intended for authorized penetration testing and security research only.

Do not use this tool on networks you do not own or have explicit permission to test.

The author (Confnameless) is not responsible for any misuse or damage caused by this program.

Unlawful interception of wireless communications is a crime in most jurisdictions.

👤 Credits
Author: Confnameless

Libraries: Scapy, Rich
