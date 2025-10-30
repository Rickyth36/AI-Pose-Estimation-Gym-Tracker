# 🏋️ BioMimic – AI Pose Estimation Gym Tracker

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![OpenCV](https://img.shields.io/badge/OpenCV-Enabled-green?logo=opencv)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Used-orange?logo=google)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Platform](https://img.shields.io/badge/Platform-Windows%20|%20macOS%20|%20Linux-lightgrey)

**BioMimic** is an AI-powered gym tracker that uses **pose estimation** to analyze workout form, count reps and provide **real-time posture feedback with alarm sound alerts** when incorrect posture is detected.  
Built using **Python, OpenCV and MediaPipe**, this project brings computer vision into fitness helping users train smarter without a personal trainer.

---

## 🚀 Demo

🎥 **Watch the Demo Video:**  
[YouTube – BioMimic Demo](https://www.youtube.com/watch?v=FxG6dp9GQDc)


---

## 💡 Features

- 🧍‍♂️ **Pose Estimation:** Detects and tracks body joints in real time.  
- 🔢 **Automatic Rep Counter:** Counts exercise reps automatically.  
- 🚨 **Audio Alert System:** Plays alarm sound when incorrect posture is detected.  
- 📊 **Live Feedback:** Displays posture alignment and rep progress.  
- ⚡ **Lightweight & Fast:** Optimized for smooth real-time performance.

---

## 🛠️ Tech Stack

| Category | Tools / Libraries |
|-----------|------------------|
| Programming Language | Python |
| Computer Vision | OpenCV |
| Pose Detection | MediaPipe |
| Math Operations | NumPy |
| Audio Feedback | playsound |
| Web UI | Flask |

---

## ⚙️ Installation & Setup

### **1️⃣ Install Python (Recommended: Python 3.10.0)**

Download Python from the official site: [https://www.python.org](https://www.python.org)  
This project recommends **Python version 3.10.0** and **pip 25.1.1 or later**.

---

### 🪟 Windows Python Installation (v3.10.0)

1. **Download Python Installer**  
   - Visit the official Python release page:  
     [Python 3.10.0](https://www.python.org/downloads/release/python-3100/)  
   - Download the **Windows Installer (64-bit)** or **Windows Installer (32-bit)** depending on your system.  
   - Save the installer to a local directory (e.g., `Downloads`).

2. **Install Python**  
   - Run the installer with **Administrative Privileges**.  
   - ✅ Check **“Add Python 3.10 to PATH”** to enable command-line access.  
   - Select **“Customize installation”** to include pip and other components.  
   - Proceed with the default installation directory:  
     ```
     C:\Users\Username\AppData\Local\Programs\Python\Python310
     ```
     (unless a custom path is required).  
   - Click **Install** and wait for the installation to complete.

3. **Verify Installation**  
   - Open **Command Prompt** or **PowerShell**.  
   - Check Python version:  
     ```bash
     python --version
     # Expected output: Python 3.10.0
     ```  
   - Check pip version:  
     ```bash
     pip --version
     # Expected output: pip 21.2.3 or later
     ```

4. **Upgrade pip (if necessary)**  
   ```bash
   python -m pip install --upgrade pip
   
### 🍎 macOS Python Installation (v3.10.0)

1. **Download Python Installer**  
   - Visit the official Python release page:  
     [Python 3.10.0](https://www.python.org/downloads/release/python-3100/)  
   - Download the **macOS 64-bit universal2 installer**.

2. **Install Python**  
   - Launch the downloaded `.pkg` installer and follow the on-screen instructions.  
   - Default installation path:  
     ```
     /Library/Frameworks/Python.framework/Versions/3.10
     ```

3. **Verify Installation**  
   - Open **Terminal** and run:  
     ```bash
     python3 --version
     # Expected output: Python 3.10.0

     pip3 --version
     # Expected output: pip 21.2.3 or later
     ```

4. **Upgrade pip (if necessary)**  
   ```bash
   python3 -m pip install --upgrade pip
5. **Troubleshooting**

     Add Python to PATH if required:
   
     ```bash
     export PATH="/Library/Frameworks/Python.framework/Versions/3.10/bin:$PATH"
     ```
     
     
     Install Xcode Command Line Tools if needed:
     ```bash
     xcode-select --install
     ```


### 🐧 Linux Python Installation (v3.10.0)

1. **Download Python Source**  
   - Visit the official Python release page:  
     [Python 3.10.0](https://www.python.org/downloads/release/python-310/)  
   - Download the Gzipped source tarball: `Python-3.10.0.tgz`  
   - Save the file to a preferred local directory (e.g., `/Downloads`)

2. **Install Build Dependencies**  

   **Debian / Ubuntu-based systems:**  
   ```bash
   sudo apt update
   sudo apt install -y build-essential libssl-dev zlib1g-dev \
   libncurses5-dev libncursesw5-dev libreadline-dev libsqlite3-dev \
   libgdbm-dev libdb5.3-dev libbz2-dev libexpat1-dev liblzma-dev tk-dev
   ```
   Red Hat / Fedora-based systems:
   ```bash
   sudo dnf groupinstall "Development Tools"
   sudo dnf install -y gcc openssl-devel bzip2-devel libffi-devel zlib-devel \
   readline-devel sqlite-devel wget make
   ```
   
   Extract and Compile Python
   ```bash
    
   cd /Downloads
   tar -xvf Python-3.10.0.tgz
   cd Python-3.10.0
   ./configure --enable-optimizations
   make -j$(nproc)
   sudo make altinstall
   Verify Installation
   ```
   
   ```bash
   python3.10 --version
   # Expected Output: Python 3.10.0
   
   pip3 --version
   # Expected Output: pip 25.1.1 or later
   Upgrade pip (if necessary)
   ```
   
   ```bash
   python3.10 -m pip install --upgrade pip
   ```
   
   Troubleshooting
   
   If python3.10 is not found, ensure /usr/local/bin is in your PATH:
   
   ```bash
   export PATH="/usr/local/bin:$PATH"
   Add this line to your shell configuration file (~/.zshrc or ~/.bash_profile)
   ```
   
   Optional: Create symbolic links for easier access (Debian/Ubuntu):
   ```bash
   sudo ln -s /usr/local/bin/python3.10 /usr/bin/python3.10
   sudo ln -s /usr/local/bin/pip3.10 /usr/bin/pip3.10
   ```

## 🏃 Running BioMimic

Once you have cloned the repository and installed dependencies, running BioMimic is simple:

### Navigate to the Project Directory
   Open a terminal or command prompt and go to the folder where you cloned the repo:
   ```bash
   cd AI-Pose-Estimation-Gym-Tracker
   ```
### Install Dependencies
   ```bash
   pip install -r requirements.txt
   ```
   If you are on macOS/Linux and pip points to Python 2, use pip3 instead: 
   ```bash
   pip3 install -r requirements.txt
   ```

 ### Launch the Application
   Run the following command in your terminal:
   ```bash
   python app.py
   ```
   Or, if python points to Python 2, use:
   ```bash
   python3 app.py
   ```
---
##Thank you for checking out **BioMimic**!  
We hope this project helps you **train smarter, track your progress, and maintain proper posture** during workouts.  
Enjoy exploring the AI-powered features and have fun improving your fitness journey! 💪
---


