# Cephas Installer

Official **APT repository** for the **Cephas command-line tool**.  
This repository helps you easily install, configure, and update the Cephas application on Debian-based systems like **Ubuntu**.

---

## 🚀 Installation & Upgrading

Please follow the instructions that match your situation.

---

### 1. For New Users (First-Time Installation)

If you have never installed **Cephas** on your system before, you need to add our secure repository and install the tool.

#### ⚡ Quick Install (Recommended)

Run this single command in your terminal to complete the installation:

```bash
curl -sS https://priv8tool.github.io/CEPHAS/public.key | sudo gpg --dearmor -o /usr/share/keyrings/cephas-archive-keyring.gpg && echo "deb [signed-by=/usr/share/keyrings/cephas-archive-keyring.gpg] https://priv8tool.github.io/CEPHAS/ ./" | sudo tee /etc/apt/sources.list.d/cephas.list > /dev/null && sudo apt update && sudo apt install cephas -y
```

---

### 2. For Existing Users (Upgrading)

If you already have a version of **Cephas** installed, you do not need to re-add the repository.  
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

---

## 📄 License

This project is licensed under the **MIT License**.
