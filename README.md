A lightweight, modern launcher hub that brings all your Minecraft launchers into one clean interface. No more digging through folders — Reforged gives you fast, unified access to CurseForge, Modrinth, Prism Launcher, ATLauncher, Technic, MultiMC, and more.

⭐ Features
Unified hub for multiple Minecraft launchers

Automatic path detection (works on ANY Windows username)

Clean, simple UI

Fully packaged Windows installer

No Python required — standalone EXE

Bundled assets + icons

Fast, lightweight, and easy to use

📥 Download
Grab the latest version here: https://github.com/vynastus10111/Reforged-Launcher/releases/tag/fix 

👉 Download Reforged 

🛠️ Installation
Download ReforgedSetup.exe from the Releases page

Run the installer

Launch Reforged from the Start Menu or Desktop

Enjoy a unified launcher experience

The installer automatically:

Installs Reforged into Program Files

Creates shortcuts

Adds an uninstaller entry in Windows Apps & Features

🔍 Supported Launchers
Reforged can detect and launch:

CurseForge

Modrinth App

Prism Launcher

ATLauncher

Technic Launcher

MultiMC

FTB App

More launchers can be added easily.

🧠 How Launcher Detection Works
Reforged uses:

python
os.path.expanduser("~")
to dynamically detect the current user’s home directory.
This ensures launcher paths work on ANY Windows machine — no hard‑coded usernames.

Paths are defined using raw f‑strings:

python
fr"{USER}\AppData\Local\Programs\CurseForge Windows\CurseForge.exe"
This avoids escape‑sequence issues and keeps the launcher portable.

🧩 Building From Source
To build your own EXE:

bash
pyinstaller --onefile --windowed --icon=reforged.ico --add-data "assets;assets" Reforged.py
To package the installer, use the included Inno Setup script:

Code
ReforgedInstaller.iss
🗺️ Roadmap
Auto‑detect installed launchers

Hide launchers that aren’t installed

Settings window for manual path overrides

Auto‑update system using GitHub Releases

Themed UI

📄 License
MIT License

👤 Author
Liam McConnell  
Creator of Reforged Launcher
