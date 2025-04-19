# Gnesyn-Node-Run-Twitter
Gensyn Node Run

1️⃣ Minimum Requirements (for personal setup):
• 💻 16 GB RAM
• ⚡ RTX 3090/4090 GPU (optional)
You can run it via:
🖥️ Your own device (if compatible)
🌐 Or a VPS

2️⃣ VPS Setup (Recommended) 

📺 Watch VPS Setup Video (linked)

🌐 Buy VPS — 
```bash https://www.vultr.com/?ref=9747762```

🪪 Create account
💳 Add credit card (only ~$2 will be deducted)
🎟 Use code: FLY300VULTR or 250VULTRFLY
💰 You’ll get $300 credit instantly

3️⃣ VPS I Bought
• 🔧 16 GB RAM
• 🧠 8 Cores
• 🕐 $160/month
• ✅ Selected Ubuntu (latest version)
Still had $140 left in credit 💸

4️⃣ Connect to VPS

📱 Use WSL on laptop or Termux on phone
🧑‍💻 Connect using:
🛜ssh linuxuser@Your_VPS_IP
🔑 Enter your VPS password

5️⃣ Install Dependencies paste the following commands 1 by 1 

sudo apt update && sudo apt install -y sudo

sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl wget screen git lsof && curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - && echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list && sudo apt update && sudo apt install -y yarn

6️⃣ Run Gensyn Node

curl -sSL https://raw.githubusercontent.com/obairnisarnajar/gensyn-crypto_kasheer/main/node.sh | bash

screen -S gensyn

cd $HOME && rm -rf gensyn-testnet && git clone https://github.com/zunxbt/gensyn-testnet.git && chmod +x gensyn-testnet/gensyn.sh && ./gensyn-testnet/gensyn.sh

➡️ To detach screen: Ctrl + A + D
➡️ To re-attach: screen -r gensyn

7️⃣ Backup Your Data (Very Important!) after DE attaching

[ -f http://backup.sh ] && rm http://backup.sh; curl -sSL -O https://raw.githubusercontent.com/obairnisarnajar/gensyn1-crypto_kasheer/main/backup.sh && chmod +x http://backup.sh && ./backup.sh

Keep your keys safe! 🔐

8️⃣ Check if Node is Running

💬 Go to: https://t.me/gensyntrackbot
Type /check your_peer_id
✅ If you see a wallet & explorer, you're good
❌ If 0x000... or blank → run commands again

9️⃣ Fix Common Errors

If you face error at the end, run:

curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash - && sudo apt install -y nodejs

cd $HOME/gensyn-testnet && ./gensyn.sh

⚠️ When it asks to create HuggingFace, type N and press enter

🧠 And that’s it!

You're now officially running a Gensyn node 💻🪂
Let it run & wait for potential rewards 🎯

