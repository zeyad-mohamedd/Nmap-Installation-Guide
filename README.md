# 👁 Nmap Installation and Usage Guide

A complete guide to installing Nmap, important addons, and practical examples for cybersecurity professionals and penetration testers.

---

## 📑 Table of Contents

| Section                          | Description                                 |
|----------------------------------|---------------------------------------------|
| [📖 What is Nmap?](#what-is-nmap) | Learn about Nmap and its key features      |
| [🛠️ How to Install Nmap](#how-to-install-nmap) | Step-by-step installation guide            |
| ├─ [🐧 Linux (Debian/Ubuntu)](#on-linux-debianubuntu) | Install on Linux systems                   |
| ├─ [🪟 Windows](#on-windows)      | Install on Windows systems                 |
| └─ [🍎 macOS](#on-macos)          | Install on macOS systems                   |
| [🔌 Important Addons and Scripts](#important-addons-and-scripts) | Enhance functionality with addons         |
| ├─ [⚙️ Nmap Scripting Engine (NSE)](#nmap-scripting-engine-nse) | Use advanced scripts                      |
| ├─ [🖼️ Zenmap](#zenmap)          | Explore the graphical user interface        |
| └─ [🛠️ Third-party Tools](#third-party-tools) | Additional tools to complement Nmap       |
| [🧪 Practical Examples](#practical-examples) | Real-world usage examples                  |
| [🔗 References](#references)     | Useful links and documentation             |

---


## 🤔 What is Nmap?

**Nmap** (Network Mapper) is a powerful open-source tool used for network discovery and security auditing. It is widely used by penetration testers, network administrators, and security professionals for tasks such as:

- 🔍 **Port scanning**
- 🖥️ **Operating system detection**
- 🛠️ **Service enumeration**
- 🛡️ **Vulnerability assessment**

For more details, visit the [official Nmap website](https://nmap.org/).

---

## 🛠️ How to Install Nmap

### 🐧 On Linux (Debian/Ubuntu)

1. **Update your system**:
   ```bash
   sudo apt update && sudo apt upgrade
   ```

2. **Install Nmap**:
   ```bash
   sudo apt install nmap -y
   ```

3. **Verify installation**:
   ```bash
   nmap --version
   ```

### 🪟 On Windows

1. **Download the installer** from the [official site](https://nmap.org/download.html).
2. **Run the installer** and follow the on-screen instructions.
3. **Verify installation**:
   - Open Command Prompt and type:
     ```cmd
     nmap --version
     ```

### 🍎 On macOS

1. **Install Homebrew** (if not already installed):
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install Nmap**:
   ```bash
   brew install nmap
   ```

3. **Verify installation**:
   ```bash
   nmap --version
   ```

---

## 🔌 Important Addons and Scripts

### ⚙️ Nmap Scripting Engine (NSE)

NSE allows advanced scanning using scripts for specific tasks. Below are some common examples:

- **Vulnerability Scan**:
  ```bash
  nmap --script vuln 192.168.1.1
  ```

- **HTTP Enumeration**:
  ```bash
  nmap --script http-enum 192.168.1.1
  ```

- **FTP Brute Force**:
  ```bash
  nmap --script ftp-brute 192.168.1.1
  ```

To explore more scripts, check the directory:
```bash
/usr/share/nmap/scripts
```

### 🖼️ Zenmap

**Zenmap** is the official GUI for Nmap, which provides a user-friendly interface for scanning.

1. **Download Zenmap** from the [official site](https://nmap.org/zenmap/).
2. **Install and launch** Zenmap.
3. Use it to visualize scan results and perform advanced scans.

### 🛠️ Third-party Tools

- **Ncat**: Networking tool for debugging and data transfer.
- **Ndiff**: A tool to compare scan results.
- **NPcap**: Packet capture driver for Windows, required for advanced features.

---

## 🧪 Practical Examples

### 🔍 Basic Scan

Scan a single IP address:
```bash
nmap 192.168.1.1
```

### 🌐 Scan a Range of IPs

```bash
nmap 192.168.1.1-50
```

### 🖥️ Detect Operating System

```bash
nmap -O 192.168.1.1
```

### 🔓 Scan for Open Ports

```bash
nmap -p 1-65535 192.168.1.1
```

### 🛡️ Run a Script

```bash
nmap --script=vuln 192.168.1.1
```

### 💾 Save Results to a File

Save the scan results in a text file:
```bash
nmap -oN scan_results.txt 192.168.1.1
```

Save the results in XML format:
```bash
nmap -oX scan_results.xml 192.168.1.1
```

---

## 🔗 References

- [🌐 Nmap Official Website](https://nmap.org/)
- [📖 Nmap Scripting Engine](https://nmap.org/book/nse.html)
- [🖼️ Zenmap GUI](https://nmap.org/zenmap/)
