# PvZ2 Gardendless - Linux AppImage Wrapper

[![Build Status](https://github.com/hthienloc/pvz2-gardendless-appimage/actions/workflows/build.yml/badge.svg)](https://github.com/hthienloc/pvz2-gardendless-appimage/actions)
[![Latest Release](https://img.shields.io/github/v/release/hthienloc/pvz2-gardendless-appimage?color=blue&label=version)](https://github.com/hthienloc/pvz2-gardendless-appimage/releases)
[![License](https://img.shields.io/github/license/hthienloc/pvz2-gardendless-appimage)](https://github.com/hthienloc/pvz2-gardendless-appimage/blob/main/LICENSE)

A high-performance standalone runner for the [PvZ2 Gardendless](https://github.com/Gzh0821/pvzge_web) web game, packaged specifically for Linux environments using Electron.

---

## 🚀 Features

* **⚡ Native Performance**: Runs as a lightweight standalone AppImage for better resource management.
* **📦 CI/CD Optimized**: Automatic builds and releases powered by GitHub Actions.
* **🛠 Integrated Hub**: Seamless support for modern AppImage managers (Gear Lever, AppImageLauncher).

## ⚡ Quick Start (CLI)

```sh
# 1. Download the AppImage
wget https://github.com/hthienloc/pvz2-gardendless-appimage/releases/download/v0.8.2/PvZ2-Gardendless-0.8.2.AppImage

# 2. Install and integrate with Gear Lever
flatpak run it.mijorus.gearlever --integrate PvZ2-Gardendless-0.8.2.AppImage --yes

# 3. Configure GitHub auto-updates
# Note: Gear Lever usually renames it to ~/AppImages/pvz2gardendless.appimage
flatpak run it.mijorus.gearlever --set-update-source ~/AppImages/pvz2gardendless.appimage \
    --manager GithubUpdater \
    repo_url=https://github.com/hthienloc/pvz2-gardendless-appimage \
    repo_filename=PvZ2-Gardendless-*.AppImage \
    allow_prereleases=false
```

## 📦 Installation

For the best experience, we recommend using [Gear Lever](https://github.com/mijorus/gearlever) (Available on Flathub) to handle system integration and automatic updates.

### Option 1: CLI (Recommended)

Follow the commands in the **Quick Start** section above.

### Option 2: GUI

1. Download the latest `.AppImage` file from the [Releases](https://github.com/hthienloc/pvz2-gardendless-appimage/releases) page.
2. Open the file with **Gear Lever** to integrate it into your application menu.

## 🔄 Automatic Updates

Gear Lever notifies you when a new version is available. To manually check and install updates for all integrated apps via CLI, use:

```sh
flatpak run it.mijorus.gearlever --update --all --yes
```

If auto-discovery fails and you need to verify or reset the update source, use the command provided in step 3 of the **Quick Start** section. You can find the exact path managed by Gear Lever using:

```sh
flatpak run it.mijorus.gearlever --list-installed
```

> [!TIP]
> **Safety First**: Unlike Docker-based solutions, AppImage updates **do not require manual backups**. Your save data and settings are stored in local configuration folders and are never touched by the update process.

---

## ❤️ Credits

* **Game Engine**: Originally developed by [Gzh0821](https://github.com/Gzh0821).
* **Linux Packaging**: Maintained by [hthienloc](https://github.com/hthienloc).
