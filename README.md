<p align="center">
  <img src="assets/icons/icon.png" width="96" alt="Auto Clicker icon">
</p>

<h1 align="center">Auto Clicker</h1>

<p align="center">
  A lightweight, high-performance auto-clicking utility for Windows.
</p>

<p align="center">
  <img alt="platforms" src="https://img.shields.io/badge/platform-Windows-blue">
  <img alt="release" src="https://img.shields.io/badge/release-v1.1.0-blue">
  <img alt="build" src="https://img.shields.io/badge/build-passing-brightgreen">
  <img alt="license" src="https://img.shields.io/badge/license-Proprietary-red">
</p>

---

## Overview

**Auto Clicker** is a small desktop app for automating mouse clicks with precise timing. It runs natively on Windows, with a clean, simple interface designed for repetitive-click use cases — testing, gaming, form filling, or any workflow where you need clicks fired on a schedule instead of by hand.

It ships as a ready-to-run app, with a global hotkey to start/stop from anywhere and a system tray presence so it stays out of your way.

## Features

- 🖱️ **Configurable click loop** — set interval (hours/minutes/seconds/milliseconds), mouse button (left/right/middle), and single or double click
- 🔁 **Flexible repeat modes** — click a fixed number of times or run until stopped
- 🎯 **Fixed or current position clicking** — click wherever the cursor is, or lock to a screen coordinate you pick visually
- ⌨️ **Global hotkey toggle** — start/stop clicking from any window with a customizable hotkey (default `F6`)
- 🧰 **System tray support** — minimize to tray or taskbar, with your preference remembered
- ⚙️ **Persistent settings** — all click parameters and preferences are saved between sessions
- 🪶 **Ultra-light footprint** — near-zero CPU and memory usage while running
- ⚡ **2x faster click and response speed** — tighter, more responsive click execution
- 🧪 **Reliability tested** — core click logic and settings behavior are covered by an internal test suite

## Showcase

> Auto Clicker in a few numbers and highlights:

| | |
|---|---|
| 🪶 **Lightweight** | Just 34MB — no background services beyond the app itself |
| ⚡ **Sub-millisecond accuracy** | Precision timing keeps click intervals tight even at high frequency |
| 🚀 **2x faster response** | Doubled click and input response speed over previous versions |
| 🔋 **Near-zero resource usage** | Minimal CPU and memory footprint, even during long sessions |
| 🔐 **Signed & verified releases** | Every release is signed to protect against tampering |

![Auto Clicker screenshot](Screenshot%202026-08-02%20170818.png)

## What's New in v1.1.0

- 🛠️ Fixed random crashes and instances where the app would get blocked without reason
- 🎨 Improved overall UI/UX for a smoother experience
- 💻 **Windows-only going forward** — macOS and Linux support has been dropped
- 📦 Reduced app size from 39MB to 34MB
- 🔋 Significantly lowered CPU and memory usage (near-zero at idle)
- ⚡ Doubled click speed and input response time
- 🚫 Permanently removed the auto-update system — see note below

> **Note:** Auto-updates have been removed permanently. Please check the [Releases](../../releases) page manually for future versions.

## Release & Support Lifecycle

| Version | Series | Status | Platforms | Notes | Released | Support Ends |
|---------|--------|--------|-----------|-------|---------------|---------------|
| 1.0.0   | Short-term | ⚫ Legacy | Windows, macOS, Linux | Initial public release | 2026/8/2 | 2026/9/3 |
| 1.1.0   | Short-term | ✅ Current | Windows | [Releases](../../releases) | 2026/8/21 | — |

**Legend:** ✅ Current • ⚫ Legacy (critical fixes only) • 🟡 End of Support (no longer supported) • 🔴 End of Life (Deprecated)

> Auto-updates have been removed as of v1.1.0. If a release ever ships with a serious issue, an advisory will be posted on the Releases page — please check manually for updates.

## Supported Platforms & Versions

| Platform | Minimum Version | Architecture | Status |
|----------|------------------|---------------|--------|
| Windows  | Windows 10 (1809+) | x64 | ✅ Fully supported |
| macOS    | — | — | ❌ No longer supported (as of v1.1.0) |
| Linux    | — | — | ❌ No longer supported (as of v1.1.0) |

> Older OS versions may still work but are untested and unsupported. If you run into issues on an unlisted Windows version, please open an issue with your OS details.

## Getting Started

### Download

Grab the latest release from the [Releases](../../releases) page:

- **Windows** — download and run the installer/executable

No additional setup, runtimes, or dependencies are required — just download and launch.

Since auto-updates have been removed, be sure to check the Releases page periodically for new versions.

## Usage

1. Launch the app.
2. Set your desired interval, mouse button, click type, and repeat mode.
3. Choose **current position** or pick a **fixed position** on screen.
4. Press **Start** (or your configured hotkey — default `F6`) to begin clicking, and press it again to stop.
5. Minimize to the tray or taskbar to keep it running in the background.

## Feedback & Issues

Found a bug or have a feature request? Please open an issue describing what happened, your OS, and the app version.

## License

This project is proprietary software — see the [LICENSE](LICENSE) file for full terms.

**In short:** you may download and use the app, but you may **not** modify it, claim ownership of it, or redistribute it as your own without prior written permission from the publisher.

## Disclaimer

Auto-clicking may violate the terms of service of some games, applications, or platforms. Use responsibly and at your own risk.
