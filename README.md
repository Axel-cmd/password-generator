# password-generator

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## 📝 Description

**password-generator** is a simple Python script that generates random and secure passwords.  
It can be used for quickly creating strong passwords for personal use, secure accounts, or any situation requiring a high-entropy password.

---

## 📦 Requirements

Before using this tool, make sure you have:

- **Python 3.8+**

---

## 🛠 Installation

Clone the repository:

```bash
git clone https://github.com/Axel-cmd/password-generator.git
cd password-generator
```

### ▶️ Run the script without typing `python` (Linux)

If you want to execute the script directly like a normal command (without typing `python` before), follow these steps:

#### 1️⃣ Add a shebang at the top of your script

At the top of your `password.py` file, make sure there is:

```python
#!/usr/bin/env python3
```

#### 2️⃣ Make the file executable

In your project folder, run:
```bash
chmod +755 password.py
```

4️⃣ Make it available everywhere

If you want to run it from anywhere in your system using only its name:

```bash
sudo cp password.py /usr/local/bin/password
```

Then simply use:

```bash
password
```

## 🧰 Command Help & Options

Below is the list of available commands and options supported by the script.

### 📌 Basic Commands

| Command | Description |
|--------|-------------|
| `password` | Generates an 8-character password using **lowercase letters only** (default). |
| `password <length>` | Generates a password with the **specified length**. |
| `password <length> [options]` | Generates a password with custom length **and optional character sets** (see options below). |

---

### 🔧 Available Options

You can add one or several options when generating a password:

| Option | Description |
|--------|-------------|
| `-u` | Adds **uppercase letters** to the password. |
| `-d` | Adds **digits (0-9)**. |
| `-s` | Adds **special characters**. |

---

### 📝 Example Usage

```bash
password                 # 8 lowercase characters (default)
password 12              # 12 lowercase characters
password 16 -u           # 16 chars, including uppercase
password 20 -ud          # 20 chars, uppercase + digits
password 24 -uds         # 24 chars, all character sets
```

