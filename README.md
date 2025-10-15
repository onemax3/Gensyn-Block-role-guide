### Gensyn BlockAssist Complete Setup Guide

> Train your AI assistant inside Minecraft and get Hugging Face + Block roles in the Gensyn ecosystem.
Works on local GPU (PC/Laptop) or OctaSpace cloud GPU.

# 📘 Introduction

BlockAssist is an AI agent that learns from your Minecraft gameplay.
It observes your actions, trains itself to assist you, and evolves with your interactions.

This guide walks you through everything:

Hugging Face token creation

OctaSpace cloud GPU deployment

Local GPU setup

Minecraft gameplay training

Discord role verification

Cleanup after use


> Follow each step carefully for a smooth setup.

# ⚙️ System Requirements

Resource	Minimum

RAM	8 GB
Disk	50–100 GB
CPU	Multi-core
GPU	✅ Required (RTX 3060+ recommended; 490+24GB minimum, 5090+32GB preferred)


# Step 1 — Create Hugging Face Account & Token

1. Go to https://huggingface.co → Sign Up

2. Fill Email, Username, Password, then click Create Account

3. Verify email via the link sent to your inbox

4. Go to Profile → Access Tokens → New Token

5. Name it BlockAssist, select Write, copy and save the token

> This token will be used later for BlockAssist deployment.

# Step 2 — Create OctaSpace Account & Deposit

1. Go to OctaSpace → Sign Up

2. Confirm email and login

3. Deposit ~0.50 USDT (BEP-20) 

> This is a low-cost investment to run BlockAssist in the cloud.


# Step 3 — Deploy BlockAssist on OctaSpace

1. Go to Marketplace → Search “Gensyn BlockAssist”

2. Choose GPU Specs: Minimum: 4090 + 24GB

Recommended: 5090 + 32GB (reduces black screen errors)

3. Click Price (~$0.50/hour)

4. Click Config → Paste your Hugging Face token → Deploy

5. Open the HTTP Service Link once session is ready

> Wait for desktop session to fully load.
Only PC/Laptop with keyboard works.


# Step 4 — Local GPU Setup (Optional)

Linux / WSL Dependencies

`sudo apt-get update -y && sudo apt-get install -y make build-essential gcc libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev curl git unzip zip mesa-utils x11-apps x11-xserver-utils libxi6 libxrender1 libxtst6 libxrandr2 libglu1-mesa libopenal1`

Install Node.js

curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt update && sudo apt install -y nodejs
node -v

Clone Repository

git clone https://github.com/gensyn-ai/blockassist.git
cd blockassist

Install Java (Minecraft required)

./setup.sh

Install pyenv + Python 3.10

curl -fsSL https://pyenv.run | bash
cat <<'EOF' >> ~/.bashrc
export PYENV_ROOT="$HOME/.pyenv"
[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init - bash)"
eval "$(pyenv virtualenv-init -)"
EOF
source ~/.bashrc
pyenv install 3.10
pip install psutil readchar rich

Start Node (Local GPU Mode)

cd ~/blockassist
source .venv/bin/activate
python3 run.py

> Re-run command if session stops or closes.




---

🎮 Step 5 — Minecraft Gameplay Training

1. Open Minecraft inside BlockAssist session


2. Press Enter → Console opens


3. Set Full Screen + 144 FPS


4. Press 1 → Equip hammer, use W/A to move


5. Break 1–2 red blocks for 3–4 minutes


6. Press Enter multiple times → Then ESC to exit



> BlockAssist learns your actions during gameplay.




---

✅ Step 6 — Discord Role Verification

Hugging Face Role

/verify huggingface

Click the link → Authorize → Role added


Block Role

/verify block

Copy your BlockAssist profile URL → Paste → Submit → Role added


> Both roles are required for full access to Gensyn ecosystem.




---

🧹 Step 7 — Cleanup

After gameplay, go to OctaSpace marketplace → Delete/Terminate your instance to avoid extra charges.



---

💡 Tips

Use high-spec GPU (5090 + 32GB) for smooth operation

Only PC/Laptop users can operate BlockAssist

Cost: ~$0.34/hour on OctaSpace

Follow every step exactly — missing roles prevent proper setup

Keyboard is mandatory; phone-only setups won’t work



---

🎯 Congratulations!

BlockAssist is now set up, trained, and integrated with Discord roles.
You can now enjoy your AI-powered Minecraft assistant and Gensyn ecosystem features.


---

✅ All commands and instructions are copy-paste ready for GitHub.


---

If you want, I can also make a “Quick Commands Section” at the very bottom, where all the commands (Linux install, Python, Git, run.py, etc.) are together in one block, so users can just copy everything in one go.

Do you want me to do that next?

