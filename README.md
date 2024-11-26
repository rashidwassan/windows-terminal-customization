# 🚀 Customize Your Windows Terminal with Starship
Transform your Windows Terminal into a professional powerhouse with **Starship** and Chocolatey! Follow this step-by-step guide to get started.

## Preview
![img](https://github.com/user-attachments/assets/59d43010-083b-45e9-aef0-aa0f7d0d2239)


---

## 🛠️ Step 1: Install Chocolatey

> **Skip this step if Chocolatey is already installed.**

1. Open **PowerShell** as Administrator.
2. Run the following command:
   ```powershell
   Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.WebClient]::new().DownloadString('https://community.chocolatey.org/install.ps1') | Invoke-Expression

## ⭐ Step 2: Install Starship

1. Install **Starship** using Chocolatey:
   ```powershell
   choco install starship -y

2. Verify the installation by checking the version:
  ```powershell
  starship --version
