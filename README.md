# StartupChannel

Automatically opens and scrolls to a specific channel when Discord starts.

## Features

- Automatically navigate to a configured channel on Discord startup
- Optional automatic scroll to bottom of the channel
- Works with both guild channels and DMs
- Configurable channel ID setting







## Installation 

### 🪄 Installation Wizard
The easiest way to install this plugin is to use the **[Plugin Installer Generator](https://bluscream-vencord-plugins.github.io)**. 
Simply select this plugin from the list and download your custom install script.

### 💻 Manual Installation (PowerShell)
Alternatively, you can run this snippet in your Equicord/Vencord source directory:
```powershell
$ErrorActionPreference = "Stop"
winget install -e --id Git.Git
winget install -e --id OpenJS.NodeJS
npm install -g pnpm
git clone https://github.com/Equicord/Equicord Equicord
New-Item -ItemType Directory -Force -Path "Equicord\src\userplugins" | Out-Null
git clone https://github.com/bluscream-vencord-plugins/blu-startupChannel.git -b "main" "Equicord\src\userplugins\blu-startupChannel"
cd "Equicord"
npm install -g pnpm
pnpm install --frozen-lockfile
pnpm build
pnpm buildWeb
pnpm inject
```
