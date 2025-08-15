### Step 1: Copy the Text Below

Copy everything inside the box:

````markdown
# Cephas Installer

Official APT repository for the Cephas command-line tool. This tool helps you easily install, configure, and update the Cephas application on Debian-based systems like Ubuntu.

---

## 🚀 Installation

Installing `cephas` is simple. Just open your terminal and run the following commands. This will add our secure APT repository and install the latest version of the tool.

### Quick Install (One-Liner)

You can run this single command to do everything at once:

```bash
curl -sS [https://priv8tool.github.io/cephas-apt-repo/public.key](https://priv8tool.github.io/cephas-apt-repo/public.key) | sudo gpg --dearmor -o /usr/share/keyrings/cephas-archive-keyring.gpg && \
echo "deb [signed-by=/usr/share/keyrings/cephas-archive-keyring.gpg] [https://priv8tool.github.io/cephas-apt-repo/](https://priv8tool.github.io/cephas-apt-repo/) ./" | sudo tee /etc/apt/sources.list.d/cephas.list > /dev/null && \
sudo apt update && \
sudo apt install cephas
````

### Step-by-Step Installation

If you prefer to run the commands one by one, follow these steps:

1.  **Add the repository's GPG key:**
    *This ensures the packages are authentic.*

    ```bash
    curl -sS [https://priv8tool.github.io/cephas-apt-repo/public.key](https://priv8tool.github.io/cephas-apt-repo/public.key) | sudo gpg --dearmor -o /usr/share/keyrings/cephas-archive-keyring.gpg
    ```

2.  **Add the repository to your sources list:**
    *This tells your system where to download the package from.*

    ```bash
    echo "deb [signed-by=/usr/share/keyrings/cephas-archive-keyring.gpg] [https://priv8tool.github.io/cephas-apt-repo/](https://priv8tool.github.io/cephas-apt-repo/) ./" | sudo tee /etc/apt/sources.list.d/cephas.list > /dev/null
    ```

3.  **Update package lists and install `cephas`:**
    *This downloads the latest package information and installs the tool.*

    ```bash
    sudo apt update
    sudo apt install cephas
    ```

-----

## 🛠️ Usage

Once installed, you can run the tool directly from your terminal:

```bash
cephas
```

-----

## ✨ Updating

To update `cephas` to the latest version, simply run the standard system update commands:

```bash
sudo apt update
sudo apt upgrade
```

-----

## 📄 License

This project is licensed under the MIT License.

````

---
### Step 2: Create the File in Your Terminal

1.  Make sure you are in your `cephas-apt-repo` directory.
2.  Run this command:
    ```bash
    cat > README.md
    ```
3.  Your terminal will now be waiting for you to input text. **Paste the text** you just copied.
4.  Press **`Ctrl + D`** to save the file and exit.

That's it! The `README.md` file is now created. You can now push it to GitHub.
````
