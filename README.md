# Nmap Installation Guide 🔍

This guide provides step-by-step instructions on how to install **Nmap** on **Kali Linux**, **Windows**, and **macOS**.

---

## **Installing Nmap on Kali Linux** 🐧

Nmap is pre-installed on most versions of Kali Linux. However, if it's missing or you want to update it, follow these steps:

### **Steps**:

1. Open the terminal. 💻
2. Update the package list:
   ```bash
   sudo apt update
   ```
3. Install Nmap:
   ```bash
   sudo apt install nmap -y
   ```
4. Verify the installation:
   ```bash
   nmap --version
   ```

---

## **Installing Nmap on Windows** 💻

To install Nmap on Windows, follow these steps:

### **Steps**:

1. Download the Nmap Windows installer from the official website: 🔗 [https://nmap.org/download.html](https://nmap.org/download.html)
2. Run the installer and follow the on-screen instructions. 🔧
   - Ensure you select the option to add Nmap to your system's PATH during installation.
3. Verify the installation:
   - Open the Command Prompt (press `Win + R`, type `cmd`, and hit Enter). 🌐
   - Run:
     ```cmd
     nmap --version
     ```

---

## **Installing Nmap on macOS** 🍏

You can install Nmap on macOS using **Homebrew**, a popular package manager for macOS.

### **Steps**:

1. Open the Terminal. 💻
2. Ensure Homebrew is installed:
   ```bash
   brew --version
   ```
   - If Homebrew is not installed, install it by running:
     ```bash
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
     ```
3. Update Homebrew:
   ```bash
   brew update
   ```
4. Install Nmap:
   ```bash
   brew install nmap
   ```
5. Verify the installation:
   ```bash
   nmap --version
   ```

---

## **Additional Resources** 🔎

- Official Nmap Documentation: [https://nmap.org/docs.html](https://nmap.org/docs.html)
- Troubleshooting and FAQs: [https://nmap.org/faq/](https://nmap.org/faq/)

Enjoy exploring networks with Nmap 🚀



