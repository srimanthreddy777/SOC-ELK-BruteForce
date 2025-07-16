# Windows Log Analysis – Brute Force & PowerShell Detection

## 📌 Project Overview

This project simulates a basic brute-force attack and PowerShell execution on a Windows machine.  
The goal is to detect and analyze these events using native Windows logs and map them to the MITRE ATT&CK framework.

---

## 🧠 What Was Done

- Simulated brute-force login failures by entering incorrect credentials
- Ran a PowerShell command (`Get-Process`)
- Opened **Event Viewer** to inspect logs
- Took screenshots for evidence
- Mapped events to MITRE ATT&CK techniques

---

## 🧪 Evidence

### 🔐 1. Brute Force (Failed Login Attempts)

- **Event ID 4625** found in Security logs
- Indicates repeated failed logon attempts (simulated)

📸 Screenshot:  
![Brute Force Logon](screenshots/01-brute-force-failed-logon.png)

> 🔎 MITRE ATT&CK: `T1110.001` – Brute Force: Password Guessing  
> [MITRE Link](https://attack.mitre.org/techniques/T1110/001/)

---

### 💻 2. PowerShell Execution

- PowerShell command manually executed
- Due to logging not enabled, `4104` not generated
- Screenshot shows PowerShell command window

📸 Screenshot:  
![PowerShell Execution](screenshots/02-powershell-command.png)

> 🔎 MITRE ATT&CK: `T1059.001` – PowerShell Execution  
> [MITRE Link](https://attack.mitre.org/techniques/T1059/001/)

---

## ✅ Conclusion

This basic detection project simulates two real-world attack behaviors:
- Brute force attempts (via Event ID 4625)
- PowerShell command execution (simulated manually)

This report shows how to detect, analyze, and map log activity to the MITRE ATT&CK framework — an essential SOC skill.

---

## 👨‍💻 Analyst: Srimanth Reddy
GitHub: [@srimanthreddy777](https://github.com/srimanthreddy777)
