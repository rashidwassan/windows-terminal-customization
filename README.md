# 🚀 Customize Your Windows Terminal with Starship
Transform your Windows Terminal into a professional powerhouse with **Starship** and Chocolatey! Follow this step-by-step guide to get started.

## Preview
![img](https://github.com/user-attachments/assets/59d43010-083b-45e9-aef0-aa0f7d0d2239)


---

## 👨‍💻 Step 0: (Optional) Install Windows Terminal
1. Download & Install Windows Terminal from the Microsoft Store using this [link](https://www.microsoft.com/store/productId/9N0DX20HK701?ocid=pdpshare).
2. Optionally, you can download preview version (that I preffer) using this [link](https://www.microsoft.com/store/productId/9N8G5RFZ9XK3?ocid=pdpshare).
3. Alternatively, if you do not have Microsoft Store on your PC, set up Windows Terminal using this [documentation](https://learn.microsoft.com/en-us/windows/terminal/install).

<br />

## 🛠️ Step 1: Install Chocolatey

> **Skip this step if Chocolatey is already installed.**

1. Open **PowerShell** as Administrator.
2. Run the following command:
   ```powershell
   Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.WebClient]::new().DownloadString('https://community.chocolatey.org/install.ps1') | Invoke-Expression

<br />


## ⭐ Step 2: Install Starship

1. Install **Starship** using Chocolatey:
   ```powershell
   choco install starship -y

2. Verify the installation by checking the version:
  ```powershell
  starship --version
   ```

<br />

## ✨ Step 3: Configure Starship Prompt

1. Navigate to `C:\Users\<YOUR_USER_CURRENT_NAME>\.config`
2. Copy the provided `starship.toml` file to the directory (or you can create one from scratch or use a [TEMPLATE](https://starship.rs/presets/).

<br />

## 🎨 Step 4: Customize Windows Terminal Profile

1. Open Windows Terminal.
2. Go to `Settings > Open JSON file` (or edit settings.json directly).
3. Copy contents from given `terminal_settings.json`, to your JSON, make sure to edit GUID before saving the file.

<br />

## 📄 Step 5: Install Fonts

1. Run `choco install firacode` to install Fira Code fonts for more polished look.
2. Alternatively, you can download the fonts of your choice from: [NERD FONTS](https://www.nerdfonts.com/font-downloads).
3. Make sure in your terminal settings, you are using same name of fonts as you install them, for example "Fira Code" or "Hack Nerd Font", that is set in config files given in this repo.

<br />

## 🌀 Step 6: Set Starship as Default Prompt
1. Make sure you have [VS Code](https://code.visualstudio.com/download) properly installed.
2. run `code $PROFILE`, command in your terminal.
3. Add the following line to your PowerShell profile ($PROFILE):
```powershell
Invoke-Expression (&starship init powershell)
```
4. Restart PowerShell to apply changes (You can simply close terminal and reopen it).

<br />

## ✅ Step 7: Test Your Setup
Open your terminal and enjoy your new look!


