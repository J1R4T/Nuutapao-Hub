================================================================================
                           NUUTAPAO HUB v4.0.0
       Official Launcher, Process Manager & Auto-Updater for Nuutapao Tools
================================================================================

[ OVERVIEW ]
Nuutapao Hub is a lightweight, frameless companion application designed to
launch, monitor, and automatically update the Nuutapao Tools suite.

It runs with ultra-fast startup (<3 seconds) and ensures you always have the 
latest version of Nuutapao Tools installed.


[ KEY FEATURES ]
1. Instant Launch & Single-Instance Focus:
   - Click "Launch Nuutapao Tools" to start the app.
   - If Nuutapao Tools is already running, Hub automatically brings its window
     to the foreground instead of opening duplicate windows.

2. Auto-Detection of Installed Tools:
   - Hub automatically detects Nuutapao Tools whether it is installed in:
     * User profile: %LOCALAPPDATA%\Programs\Nuutapao Tools\
     * System 64-bit: C:\Program Files\Nuutapao Tools\
     * System 32-bit: C:\Program Files (x86)\Nuutapao Tools\
     * Local Dev/Unpacked builds in the dist/ folder

3. Seamless GitHub Releases Auto-Updater:
   - Automatically checks GitHub for newer releases.
   - Reads official release notes and changelogs.
   - Downloads updates directly inside Hub with a real-time progress bar,
     transfer speed indicator (MB/s), and percentage tracker.
   - Automatically runs the new installer when the download finishes.

4. Modern Frameless Glassmorphic Interface:
   - Clean dark-mode aesthetic with custom titlebar controls (Minimize, 
     Maximize/Restore, and Close).
   - Responsive and lightweight.


[ HOW TO RUN ]
- From Executable (.exe):
  Double-click "Nuutapao Hub.exe"

- From Source / Development:
  Open terminal in the project root and run:
    npm run hub

- To build standalone "Nuutapao Hub.exe":
    npm run build:hub


[ SYSTEM REQUIREMENTS ]
- Operating System: Windows 10 or Windows 11 (64-bit)
- Memory: 512 MB RAM or higher
- Internet connection (required for GitHub update checking and downloads)


[ FILE STRUCTURE ]
hub/
  ├── assets/          - Application icons and mascots
  ├── index.html       - Hub interface layout
  ├── main.js          - Electron background process & update engine
  ├── preload.js       - Secure IPC bridge
  ├── app.js           - Frontend logic & download progress handler
  ├── style.css        - Glassmorphic dark styling
  ├── README.md        - Markdown documentation
  └── README.txt       - Plain-text documentation (this file)


[ REPOSITORY & UPDATES ]
- GitHub Repository: https://github.com/J1R4T/Nuutapao-Tools
- Author: J1R4T
- License: MIT License

================================================================================
            Thank you for using Nuutapao Tools & Nuutapao Hub!
================================================================================
