# WiFi Password Extractor (Windows)

This Python script allows you to extract saved Wi-Fi network names (SSIDs) and their corresponding passwords from a Windows machine. It utilizes Windows command-line utilities to access the network profiles stored on the system.

##  Features

- Lists all saved Wi-Fi profiles on your system.
- Extracts and displays the passwords for each network (if available).
- Simple and lightweight Python script — no external libraries needed.

##  How It Works

The script uses the following command-line operations under the hood:
- `netsh wlan show profiles` — to get the list of saved networks.
- `netsh wlan show profile name="SSID" key=clear` — to extract the key (password) for each profile.

##  Getting Started

### Prerequisites

- Python 3.x installed on a Windows system
- Administrator privileges (required to access password info)

### Running the Script

```bash
python wifi_pass.py
