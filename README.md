# 🚀 Installation & Upgrading

Please follow the instructions that match your situation.

---

### 1. Brand New VPS Server (First-Time Installation)

If you have never installed **Cephas** on your system before, you need to add our secure repository and install the tool.

#### ⚡ Quick Install (Recommended)

Run this single command in your terminal to complete the installation:

```bash
curl -sS https://priv8tool.github.io/CEPHAS/public.key | sudo gpg --dearmor -o /usr/share/keyrings/cephas-archive-keyring.gpg && echo "deb [signed-by=/usr/share/keyrings/cephas-archive-keyring.gpg] https://priv8tool.github.io/CEPHAS/ ./" | sudo tee /etc/apt/sources.list.d/cephas.list > /dev/null && sudo apt update && sudo apt install cephas -y
```

---

### 2. For Existing Vps (Upgrading)

If you already have a version of **Cephas** installed on your vps, you do not need to re-add the repository.  
To upgrade to the latest version, simply run:

```bash
sudo apt update
sudo apt upgrade
```

---

## 🛠️ Usage

Once installed, you can run the tool directly from your terminal:

```bash
cephas
```
