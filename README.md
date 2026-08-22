# 🚀 My Windows 10 Setup 

![Windows 10](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)

My personal Windows 10 post-installation setup repository! 

Reinstalling Windows can be a tedious process. This repository contains the scripts, configurations, and tweaks I use to automate my Windows 10 setup, debloat the system, and install my essential tools—from web and Python environments to powerful terminal utilities—in one go.

## ✨ Features

* **⚡ Automated Software Installation:** Quickly installs essential apps, browsers, and developer tools.
* **🧹 System Optimization & Debloat:** Removes unnecessary built-in Windows telemetry and bloatware to keep the system fast and clean.
* **👨‍💻 Development Ready:** Pre-configures environments for Web Development and Python out of the box.
* **⌨️ Terminal Power-Ups:** Integrates fast CLI search tools like `fzf` and `fd` for a frictionless command-line experience.
* **📝 Knowledge Management:** Sets up digital brain tools including Obsidian and Notion.

## 📦 What gets installed?

Here is a breakdown of the primary software and tools included in this setup:

### 💻 Development Tools
* **Languages:** Python 3.x, Node.js
* **Editors & IDEs:** Visual Studio Code
* **Version Control:** Git, GitHub Desktop

### ⌨️ Terminal & CLI Utilities
* **Terminal:** Windows Terminal
* **Fuzzy Finder:** `fzf` (Command-line fuzzy finder)
* **File Search:** `fd` (Simple, fast, and user-friendly alternative to `find`)

### 🧠 Productivity & Note-Taking
* Obsidian
* Notion

### 🛠 Utilities & Media
* **Browsers:**  Helium / Waterfox
* **Media:** VLC, Spotify
* **Misc:** 7-Zip, FLowlauncher

---

## 🔎 Spotlight: `fzf` & `fd`

If you are new to these CLI tools, they will completely change how you navigate the terminal. Here is a quick breakdown of how they work and how to use them in Windows.

### ⚡ `fd` (Fast File Search)
`fd` is a ridiculously fast, user-friendly alternative to the traditional `find` command (or `Get-ChildItem` in PowerShell). 
* **Why use it?** It colorizes your output, automatically respects your `.gitignore` files (so you never waste time searching inside `node_modules` or `.git`), and uses smart case-sensitivity. 
* **Installation:** Usually installed via `winget install sharkdp.fd` or `scoop install fd`.
* **How to use it:** Simply type `fd <search-term>` in your terminal to instantly find any file or folder in your current directory.

### 🔍 `fzf` (Fuzzy Finder)
`fzf` is an interactive command-line filter that can be used with any list (files, command history, processes, git branches). 
* **Why use it?** It allows you to quickly filter through massive lists by just typing partial names. When integrated with PowerShell (via modules like `PSFzf`), it gives you magical shortcuts.
* **Installation:** Usually installed via `winget install junegunn.fzf` or `scoop install fzf`.
* **How to use it:** 
  * You can pipe any command into it to filter results: `ls | fzf`
  * With PowerShell integration, you can press `Ctrl + R` to quickly fuzzy-search your command history, or `Ctrl + T` to find and select files directly into your current command.

---

## 🚀 Usage

> **⚠️ Disclaimer:** Please review the scripts before running them on your own machine. Some tweaks modify the registry and system settings. Run at your own risk!

1. **Open PowerShell as Administrator.**
2. Clone this repository to your local machine:
   ```powershell
   git clone [https://github.com/A44Di/My-Win10-Setup.git](https://github.com/A44Di/My-Win10-Setup.git)
   cd My-Win10-Setup
