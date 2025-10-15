# 🧠 Gensyn BlockAssist Complete Guide (Local + OctaSpace)

✨ Train your own AI assistant inside Minecraft and earn the **BLOCK Role** in Gensyn’s ecosystem.

---

## 📘 Introduction

**BlockAssist** is an AI agent that learns from your actions inside Minecraft.  
It observes your gameplay, learns how to assist you, and evolves with your interactions — showing an early form of assistance learning in action.

This guide walks you through everything — from setup to training — whether you’re using your **own GPU (local)** or **OctaSpace (cloud GPU)**.

---

## ⚙️ System Requirements

| Resource | Minimum |
|-----------|----------|
| RAM | 8 GB |
| Disk Space | 50–100 GB |
| CPU | Multi-core |
| GPU | ✅ Required (RTX 3060 or higher recommended) |
| VPS | ❌ Not supported (CPU-only VPS won’t work) |


## 🧰 Step 1 — Install Dependencies

### 🐧 Linux / WSL (Windows Subsystem)

```bash
sudo apt-get update -y && sudo apt-get install -y make build-essential gcc libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev libncursesw5-dev xz-utils tk-dev libxml2-dev \
libxmlsec1-dev libffi-dev liblzma-dev curl git unzip zip mesa-utils x11-apps x11-xserver-utils \
libxi6 libxrender1 libxtst6 libxrandr2 libglu1-mesa libopenal1
```

## Step 2 — Install Node.js

bash
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash - && sudo apt update && sudo apt install -y nodejs node -v
