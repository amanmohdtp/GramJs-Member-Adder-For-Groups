<p align="center">
  <img src="https://media.giphy.com/media/3o7TKMt1VVNkHV2PaE/giphy.gif" width="120" />
</p>

<h1 align="center">🚀 GramJS Telegram Member Adder Bot</h1>

<p align="center">
  <b>A powerful GramJS-based Telegram bot to invite users into groups using Telegram IDs</b><br>
  Optimized for <b>Termux (Android)</b> & <b>Linux</b> using <b>Yarn</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-v18+-green">
  <img src="https://img.shields.io/badge/GramJS-Latest-blue">
  <img src="https://img.shields.io/badge/Platform-Termux%20%7C%20Linux-orange">
  <img src="https://img.shields.io/badge/Status-Stable-success">
</p>

---

## ✨ Features

✅ Add users to Telegram groups using **Telegram IDs**  
✅ Smart **delay & daily limit** protection  
✅ Interactive **CLI command system**  
✅ Works smoothly on **Android (Termux)**  
✅ No bot token required (user session based)  
✅ Session saved locally for reuse  

---

## 📦 Prerequisites

Make sure you have the following:

- 📱 Telegram account  
- 🔑 Telegram API credentials  
  - `apiId`
  - `apiHash`
  - Get them from 👉 https://my.telegram.org  
- 🖥 Termux (Android) or any Linux shell  
- 🟢 Node.js **v18+ recommended**  
- 🧶 Yarn package manager  

---

## 🚀 Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/amanmohdtp/GramJs-Member-Adder-For-Groups.git
cd gramjs-bot-id
2️⃣ Install Dependencies (Yarn)
Copy code
Bash
yarn install --ignore-optional
⚠️ Why --ignore-optional?
Some native modules (bufferutil, utf-8-validate) fail in Termux.
This flag ensures smooth installation.
3️⃣ Configure the Bot
Edit config.json:
Copy code
Json
{
  "apiId": 123456,
  "apiHash": "yourapihash_here",
  "session": "",
  "targetGroup": "https://t.me/yourgroup",
  "delay": 10000,
  "dailyLimit": 50
}
🔧 Configuration Guide
Field
Description
apiId
Telegram API ID
apiHash
Telegram API Hash
session
Auto-generated after login
targetGroup
Group invite link
delay
Delay between adds (ms)
dailyLimit
Max adds per day
▶️ Run the Bot
Start the bot with:
Copy code
Bash
yarn start
🔐 On first run, you’ll be asked for:
Phone number
Login code
2FA password (if enabled)
Session will be saved automatically.
💻 Bot Commands (CLI)
Once inside the bot prompt (>):
📥 Save Telegram IDs
Copy code
Text
/saveid
Paste IDs one per line, then end with a single dot:
Copy code
Text
123456789
987654321
.
➕ Add Users to Group
Copy code
Text
/add
📊 Check Status
Copy code
Text
/status
❌ Exit Bot
Copy code
Text
/exit
⚠️ Important Notes
⚠️ Only valid Telegram IDs are processed
⚠️ Users with strict privacy settings may be skipped
⚠️ Daily limit prevents Telegram rate-limits & bans
⚠️ Session data is stored locally in config.json
🛠 Development Info
🟢 Built with Node.js
📦 Powered by GramJS
🧶 Dependency management via Yarn
💻 Cross-platform:
Linux
macOS
Windows
Android (Termux)
🎬 Preview (Animation)
�
￼ 

⭐ Support
If this project helped you:
⭐ Star the repository
🧑‍💻 Contribute improvements
🐞 Report issues
