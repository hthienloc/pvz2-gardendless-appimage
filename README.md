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

## 📦 Installation

For the best experience, we recommend using an AppImage manager to handle system integration and automatic updates.

1. Install [Gear Lever](https://github.com/mijorus/gearlever) (Available on Flathub).
2. Download the latest `.AppImage` file from the [Releases](https://github.com/hthienloc/pvz2-gardendless-appimage/releases) page.
3. Open the file with **Gear Lever** to integrate it into your application menu.

## 🔄 Automatic Updates

If auto-discovery fails in **Gear Lever**, apply the following settings in **Update management**:

* **Source**: `Github`
* **Repo URL**: `https://github.com/hthienloc/pvz2-gardendless-appimage`
* **Release file name**: `PvZ2-Gardendless-*.AppImage`
* **Allow pre-releases**: Disabled

> [!TIP]
> **Safety First**: Unlike Docker-based solutions, AppImage updates **do not require manual backups**. Your save data and settings are stored in local configuration folders and are never touched by the update process.

---

## ❤️ Credits

* **Game Engine**: Originally developed by [Gzh0821](https://github.com/Gzh0821).
* **Linux Packaging**: Maintained by [hthienloc](https://github.com/hthienloc).
