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

#### 📝 Step-by-Step Installation

If you prefer to run the commands individually, follow these steps:

**1. Add the repository's GPG key**  
*(This ensures the packages you download are authentic.)*

```bash
curl -sS https://priv8tool.github.io/CEPHAS/public.key | sudo gpg --dearmor -o /usr/share/keyrings/cephas-archive-keyring.gpg
```

**2. Add the repository to your system's sources**  
*(This tells your system where to find the cephas package.)*

```bash
echo "deb [signed-by=/usr/share/keyrings/cephas-archive-keyring.gpg] https://priv8tool.github.io/CEPHAS/ ./" | sudo tee /etc/apt/sources.list.d/cephas.list > /dev/null
```

**3. Update package lists and install Cephas:**

```bash
sudo apt update
sudo apt install cephas
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
