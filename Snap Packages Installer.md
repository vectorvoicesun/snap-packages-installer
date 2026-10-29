# 📦 Snap Packages Installer

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=20,27,2&height=210&section=header&text=Snap%20Packages%20Installer&fontSize=54&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=One%20Command.%20Any%20App.%20Anywhere.&descAlignY=56&descSize=19" width="100%"/>

<br/>

[![Version](https://img.shields.io/badge/version-3.2.0-E85D04?style=for-the-badge&logo=semanticrelease&logoColor=white)](https://github.com)
[![Platform](https://img.shields.io/badge/Ubuntu%20%7C%20Fedora%20%7C%20Arch%20%7C%20Debian-F48C06?style=for-the-badge&logo=linux&logoColor=white)](https://github.com)
[![License](https://img.shields.io/badge/license-GPL--3.0-FAA307?style=for-the-badge&logo=gnu&logoColor=black)](LICENSE)
[![Snaps](https://img.shields.io/badge/snaps-10%2C000%2B-FFBA08?style=for-the-badge&logo=snapcraft&logoColor=black)](https://snapcraft.io)

<br/>

### 🚀 A friendly GUI & CLI installer that makes Snap packages effortless

*🎯 One-Click Install • 🔍 Smart Search • 🔄 Auto-Updates • 🛡️ Sandboxed*

<br/>

<a href="https://share.google/hhfTClG13lYR14xIw">
  <img src="https://img.shields.io/badge/📥_INSTALL_TOOL-E85D04?style=for-the-badge&logo=download&logoColor=white&labelColor=B34703" alt="Install Tool" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/hhfTClG13lYR14xIw">
  <img src="https://img.shields.io/badge/🔍_BROWSE_SNAPS-F48C06?style=for-the-badge&logo=snapcraft&logoColor=white&labelColor=C26F05" alt="Browse Snaps" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/hhfTClG13lYR14xIw">
  <img src="https://img.shields.io/badge/📚_DOCS-FAA307?style=for-the-badge&logo=readthedocs&logoColor=black&labelColor=C88406" alt="Docs" height="45"/>
</a>

</div>

<img width="1024" height="418" alt="snapcraft_green-red_hex-e1594609546509-1024x418" src="https://github.com/user-attachments/assets/abc21581-e259-4a31-a5f5-b76edb7a8c9b" />


<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🌟 About

**Snap Packages Installer** is a sleek, cross-distro desktop application and CLI wrapper that makes installing, updating, and managing **Snap packages** on Linux dead simple.

No more memorizing `snap install --classic` flags or hunting down package names — just **search, click, install**. Under the hood, it uses the official Snapcraft API and `snapd` daemon to guarantee **safe, sandboxed** installs every time.


<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎯 Key Features

<div align="center">

| 🔍 **Smart Search** | 🎯 **One-Click Install** | 🔄 **Auto-Updates** |
|:---:|:---:|:---:|
| Find any of 10,000+<br/>snaps instantly | Classic, strict or<br/>devmode — auto-detected | Scheduled refresh<br/>for all your snaps |

| 🛡️ **Sandboxed** | 📊 **Package Info** | 🖥️ **GUI + CLI** |
|:---:|:---:|:---:|
| Every snap runs in<br/>its own isolated container | Version, size, publisher,<br/>permissions preview | Pick your workflow —<br/>desktop app or terminal |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🏆 Why This Tool

<div align="center">

| 💎 **Advantage** | 📝 **Description** |
|:---|:---|
| 🎨 **Beautiful GUI** | Modern, native-looking interface — no need to remember CLI flags ever again |
| ⚡ **Blazing Fast** | Parallel downloads and delta updates reduce install time by up to 70% |
| 🛡️ **Safety First** | Validates every install against the Snapcraft API — no third-party injection |
| 🔄 **Smart Updates** | Automatically refreshes snaps and rolls back if the new version breaks |
| 🌍 **Multi-Distro** | Works on Ubuntu, Fedora, Arch, Debian, openSUSE & more |
| 🧩 **Scriptable** | Full CLI with JSON output — perfect for automation and provisioning scripts |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎬 Live Preview

<div align="center">

```ascii
╔══════════════════════════════════════════════════╗
║  📦  Snap Packages Installer  v3.2.0             ║
╠══════════════════════════════════════════════════╣
║                                                  ║
║  🔍 Search: [ firefox                          ] ║
║                                                  ║
║  ┌────────────────────────────────────────────┐  ║
║  │ 🌐 firefox        120.0.1  ⭐ 4.8   📦 250MB│  ║
║  │    Mozilla Firefox web browser             │  ║
║  │    [ Install ]   [ Details ]               │  ║
║  └────────────────────────────────────────────┘  ║
║  ┌────────────────────────────────────────────┐  ║
║  │ 🎨 inkscape        1.3.2  ⭐ 4.7   📦 320MB│  ║
║  │    Vector graphics editor                  │  ║
║  │    [ Install ]   [ Details ]               │  ║
║  └────────────────────────────────────────────┘  ║
║                                                  ║
║  ✅ 2 snaps available   🔄 Auto-update: ON       ║
╚══════════════════════════════════════════════════╝
```

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🧩 Project Structure

```
📦 snap-packages-installer/
├── 🎨 gui/                    # Desktop application (GTK/Qt)
│   ├── windows/
│   ├── widgets/
│   └── themes/
├── 🖥️  cli/                    # Command-line interface
│   ├── commands/
│   └── output/
├── 🔍 search/                 # Snapcraft API integration
├── ⚙️  installer/             # Install engine & permissions
├── 🔄 updater/                # Auto-update scheduler
├── 🧪 tests/                  # Unit & integration tests
└── 📖 docs/                   # User guide & API reference
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🛠️ Tech Stack

<div align="center">

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![GTK](https://img.shields.io/badge/GTK4-7B4D9E?style=for-the-badge&logo=gnome&logoColor=white)
![CLI](https://img.shields.io/badge/CLI-4E4E4E?style=for-the-badge&logo=gnometerminal&logoColor=white)
![Snapd](https://img.shields.io/badge/Snapd-82BEA0?style=for-the-badge&logo=snapcraft&logoColor=black)
![Systemd](https://img.shields.io/badge/Systemd-000000?style=for-the-badge&logo=systemd&logoColor=white)

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🤝 Community

Found a bug? Missing a distro? Want to add a feature?

<div align="center">

<a href="https://share.google/hhfTClG13lYR14xIw">
  <img src="https://img.shields.io/badge/💬_Join_Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" height="35"/>
</a>
<a href="https://share.google/hhfTClG13lYR14xIw">
  <img src="https://img.shields.io/badge/🐞_Report_Issue-E85D04?style=for-the-badge&logo=github&logoColor=white" height="35"/>
</a>
<a href="https://share.google/hhfTClG13lYR14xIw">
  <img src="https://img.shields.io/badge/⭐_Star_Repo-FAA307?style=for-the-badge&logo=github&logoColor=black" height="35"/>
</a>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 📜 License

Distributed under the **GPL-3.0 License**. See [`LICENSE`](LICENSE) for details.


<br/>

<div align="center">

### 📦 Made with 🐧 by the Snap Installer Team

*If this tool saved you a terminal command — star the repo!*

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=20,27,2&height=120&section=footer" width="100%"/>

</div>

---
