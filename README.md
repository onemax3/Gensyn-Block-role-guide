# Gensyn BlockAssist — Complete Step-by-Step Guide (GPU + OctaSpace Users)

Welcome to the simplest guide to deploy **BlockAssist** and earn your **BLOCK role** in the Gensyn Discord.  
Follow these simple steps carefully — whether you’re using your own GPU or **OctaSpace Cloud GPU**, you’ll be verified and get the role in 5minutes.

### Recommended Node Specs

| Resource | Minimum | Recommended |
|-----------|----------|--------------|
| **CPU** | 6 cores | 8+ cores |
| **RAM** | 16 GB | 32 GB |
| **Storage** | 100 GB | 100+ GB |
| **GPU** | RTX 3060+ | RTX 4070 / 5090 (32GB) |

## 2. Create a Hugging Face Account

1. Go to [https://huggingface.co](https://huggingface.co)  
2. Click **Sign Up** and create a new account (use a new email if needed).  
3. Verify your email from the link sent to your inbox.  
4. Once logged in:  
   - Click your **Profile Icon → Settings → Access Tokens**  
   - Click **New Token** → select **Write access** → name it (e.g., `BlockAssist`) → **Create Token**  
   - **Save this token** — you’ll need it later.

## 🖥️ 3. Choose Your Setup Method

You can run **BlockAssist** in two ways 👇

### Option A: Use OctaSpace (Cloud GPU — easiest)

Perfect if you don’t have a powerful local GPU.

1. Visit [OctaSpace](https://octaspace.com) and **Sign Up** with your email.  
2. Deposit **~$0.50 USDT (BEP-20)** into your wallet.  
3. Go to the **Marketplace** tab.  
4. Search **"Gensyn BlockAssist"** and open it.  
5. Choose a GPU — preferably **RTX 5090 (32GB)** to avoid lag or black screens.  
6. Click **Configure**, paste your **Hugging Face Token** in the token field, and click **Deploy**.  
7. Wait for the service status to show **Configured**.

Once configured:
- Go to **Services → HTTP Service Link** → open your desktop session.  
- Wait for the window to load (can lag for a few seconds).  
- Click **Start → Konsole (terminal)**.

### Option B: Use Your Own GPU (Local Setup)

If you already have a powerful GPU (RTX 3060 or higher):

1. Open your **Terminal** (Linux/Mac) or **PowerShell** (Windows).  
2. Run the **BlockAssist installation command:**

    ```bash
    bash <(curl -fsSL https://raw.githubusercontent.com/HustleAirdrops/Gensyn-Block-Role-Guide/main/block.sh)
    ```

3. When prompted, type `y` and press **Enter**.  
4. After installation completes, run:

    ```bash
    cd ~/blockassist && source .venv/bin/activate && python3 run.py
    ```

5. Enter your **Hugging Face Token** when asked.  
6. Wait for the **Minecraft windows** to open automatically.

## 4. Training Session (Minecraft Phase)

Once BlockAssist starts:

1. Two windows will open — **Minecraft (1.11.2)** and a **console**.  
2. In Minecraft:  
   - Press **Enter** to start.  
   - Use **W / A / S / D** to move.  
   - Press **1** to equip the tool.  
   - Break red blocks for **2–4 minutes**.  
3. After playing:  
   - Press **Enter** in the console **3 times**.  
   - Wait for confirmation of successful training submission.  

✅ You’ve now trained your model!

## 5. Retrieve Model Link

1. Go to your **Hugging Face Profile → Models**.  
2. Copy your **Model URL** (e.g., `https://huggingface.co/username/modelname`).

## 6. Claim Roles on Discord

Join the [Gensyn Discord](https://discord.gg/gensyn) and complete these:

### Step 1 — Verify Hugging Face Role
1. Go to **#link-for-access** channel.  
2. Type `/verify-huggingface`.  
3. Paste your **Hugging Face Token** → click **Authorize**.  
4. You’ll now receive the **Hugging Face** role.

### Step 2 — Verify Block Role
1. Go to **#the-swarm** channel.  
2. Type `/verify-block`.  
3. Paste your **Model URL**.  
4. Submit — you’ll receive the **BLOCK** role.

## 7. (Optional) Delete Instance (OctaSpace Users)

To avoid extra charges:

1. Go back to **OctaSpace Marketplace**.  
2. Find your running instance.  
3. Click **Terminate/Delete**.

## 🏁 You’re Done!

🎉 Congratulations — you’ve successfully deployed **Gensyn BlockAssist**, trained your model, and claimed your Discord roles!  
If you faced any issues, check the official [Gensyn Discord](https://discord.gg/gensyn) for support.
