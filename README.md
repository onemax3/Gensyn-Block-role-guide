# Gensyn Node + Swarm + BlockAssist — Complete Role Guide

Welcome to the all-in-one guide to earn your **SWARM**, **BLOCK**, and **Hugging Face** roles in Gensyn Discord.  
Follow this step-by-step — even beginners can get it running in under an hour!

## ⚙️ 1. Node Setup (Base Node Start)

This is your main command to start the Gensyn Node.  
It automatically installs all dependencies and configures your local environment.

### One-Command Node Installation
```bash
    cd ~/blockassist && source .venv/bin/activate && python3 run.py
    ```

💡 If it gets terminated, just restart your terminal and run the same command again.
If it still fails wait a few minutes and retry (network sync delay).

After setup completes, your node will start automatically.

2. SWARM Role Setup

Once your node runs, connect your Telegram to get Swarm notifications and Discord role verification.

🧰 Step 1 — Install Go

Linux / WSL:

cd ~
wget https://go.dev/dl/go1.24.0.linux-amd64.tar.gz
sudo rm -rf /usr/local/go
sudo tar -C /usr/local -xzf go1.24.0.linux-amd64.tar.gz
echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.bashrc
echo 'export GOPATH=$HOME/go' >> ~/.bashrc
echo 'export PATH=$PATH:$GOPATH/bin' >> ~/.bashrc
source ~/.bashrc
go version

macOS:

brew install go

🤖 Step 2 — Create Telegram Bot

1. Go to @BotFather on Telegram.

2. Send /newbot → set name and username.

3. Copy your Bot Token (looks like 84100000:AAGIxxxxxx...).

4. Don’t share it with anyone.

Step 3 — Get Your Chat ID

1. Send a message to your bot.

2. Open this URL in your browser (replace with your bot token):

https://api.telegram.org/botYOUR_BOT_TOKEN/getUpdates


3. Find "chat":{"id":123456789} → That’s your Chat ID.


> 💡 If it shows "result":[], just send a message to your bot and refresh the link.


⚙️ Step 4 — Install & Configure GSwarm

go install github.com/Deep-Commit/gswarm/cmd/gswarm@latest
gswarm --version

Now configure it:

gswarm

Then enter:

Your Bot Token (from step 2)

Your Chat ID (from step 3)

Your EOA address (from Gensyn Dashboard)

Step 5 — Link Discord & Telegram

1. In Gensyn Discord, open the #swarm-link channel.
Type:

/link-telegram

→ Copy the code you get.

2. Go to your Telegram bot and type:

/verify your_code_here

✅ You’ll instantly get the SWARM Role!


3. BLOCK Role Setup (BlockAssist)

You can earn the BLOCK role by training the AI agent via OctaSpace (Cloud GPU) or your own GPU.

 Option A — Use OctaSpace (Cloud GPU, easiest)

Perfect if you don’t have a powerful GPU locally.

1. Visit https://octaspace.network → Sign Up

2. Deposit around $0.5 USDT (BEP-20) into your wallet

3. Go to Marketplace → search “Gensyn BlockAssist”

4. Select GPU → RTX 5090 (32GB) recommended

5. Click Configure → paste your Hugging Face Token → click Deploy

6. Wait until status = Configured

Then:

Go to Services → HTTP Service Link

Wait for desktop session to load

Click Start → Konsole (terminal)

Option B — Use Your Own GPU (Local Setup)

If you have a local GPU (RTX 3060 or higher):

1. Open your Terminal (Linux/Mac) or PowerShell (Windows)

2. Run this:

bash <(curl -fsSL https://raw.githubusercontent.com/HustleAirdrops/Gensyn-Block-Role-Guide/main/block.sh)

3. When prompted → type y and press Enter

4. After install:

cd ~/blockassist && source .venv/bin/activate && python3 run.py

5. Enter your Hugging Face Token when asked

6. Wait for Minecraft windows to open automatically


Training Session (Minecraft Phase)

Once BlockAssist starts:

1. Two windows open → Minecraft (1.11.2) & Console

2. In Minecraft:

Press Enter to start

Use W / A / S / D to move

Press 1 to equip tool

Break red blocks for 2-4 minutes

3. After training:

Press Enter in console 3 times

Wait for training submission confirmation


✅ You’ve now trained your model!


Retrieve Model Link

1. Go to your Hugging Face Profile → Models

2. Copy your Model URL
(e.g., https://huggingface.co/username/modelname)

Claim BLOCK Role on Discord

1. Join Gensyn Discord

2. Go to #the-swarm

3. Type:

/verify-block

4. Paste your Model URL → Submit
✅ You’ll receive the BLOCK Role


4. (Optional) Stop / Restart / Delete

Stop node

pkill -f blockassist

Restart node

bash <(curl -fsSL https://raw.githubusercontent.com/HustleAirdrops/Gensyn-Block-Role-Guide/main/block.sh)

Delete OctaSpace instance (to save cost)

1. Go to OctaSpace → Marketplace

2. Find your active instance

3. Click Terminate/Delete

🏁 Done!
