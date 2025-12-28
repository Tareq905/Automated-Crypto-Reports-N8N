# 🔐 Keylogging Simulation & Detection System  
**Cybersecurity Awareness Project (Red Team & Blue Team Concepts)**

---

## 📌 Project Overview
This project is a **Keylogging Simulation & Detection System** designed to demonstrate both **attacker (red team)** and **defender (blue team)** perspectives in cybersecurity.

The system is built strictly for **educational, academic, and awareness purposes**. It does **not perform real keylogging** or any malicious activity. Instead, it simulates attacker behavior in a safe manner and showcases how defensive mechanisms can be used to detect suspicious activities.

This project helps learners and security enthusiasts understand:
- How keylogging-style threats conceptually work
- How defensive monitoring can identify suspicious processes
- The importance of ethical and responsible security research

---

## 🏗️ System Architecture & Modes

The project operates in two clearly separated modes to maintain safety and clarity.

---

### 1️⃣ Simulation Mode (Red Team Perspective)
This mode **simulates** how attackers might attempt to gather information from a system.

**Key Characteristics:**
- No real keystrokes are captured
- All keystrokes are randomly generated and simulated
- Used only to demonstrate attacker techniques conceptually

**Simulation Capabilities:**
- Collects basic system information (OS, machine type, processor, hostname)
- Takes a screenshot of the current screen
- Generates **fake keystroke logs** using random characters

---

### 2️⃣ Detection Mode (Blue Team Perspective)
This mode demonstrates **defensive security practices** by scanning the system for suspicious activity.

**Detection Capabilities:**
- Scans running processes
- Identifies suspicious process names commonly associated with keylogging behavior (e.g., `keyboard`, `pynput`)
- Helps demonstrate early detection techniques used in endpoint security

---

## ✨ Features
- System information collection (OS, hardware, hostname)
- Screenshot capture
- Simulated keystroke generation (safe & non-invasive)
- Suspicious process detection
- Simple and user-friendly menu-driven interface
- Clear separation between simulation and detection logic

---

## ▶️ Usage Guide

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/cybersecurity-awareness-tool.git

cd cybersecurity-awareness-tool

