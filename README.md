<p align="center">
  <img src="assets/icons/icon.png" width="96" alt="Auto Clicker icon">
</p>

<h1 align="center">Auto Clicker</h1>

<p align="center">
  A lightweight, cross-platform, configurable auto-clicking utility for Windows, macOS, and Linux.
</p>

<p align="center">
  <img alt="platforms" src="https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-blue">
  <img alt="python" src="https://img.shields.io/badge/python-3.10%2B-blue">
  <img alt="build" src="https://img.shields.io/badge/build-passing-brightgreen">
  <img alt="license" src="https://img.shields.io/badge/license-TBD-lightgrey">
</p>

---

## Overview

**Auto Clicker** is a small desktop app for automating mouse clicks with precise timing. It's built with PyQt6 for the UI and [`pynput`](https://pynput.readthedocs.io/) for cross-platform input injection, so the same codebase runs on Windows, macOS, and Linux (including Chrome OS via Crostini) without platform-specific forks.

It's designed for repetitive-click use cases — testing, gaming, form filling, or any workflow where you need clicks fired on a schedule instead of by hand — with a clean UI, a global hotkey to start/stop from anywhere, and a system tray presence so it stays out of your way.

## Features

- 🖱️ **Configurable click loop** — set interval (hours/minutes/seconds/milliseconds), mouse button (left/right/middle), and single or double click
- 🔁 **Flexible repeat modes** — click a fixed number of times or run until stopped
- 🎯 **Fixed or current position clicking** — click wherever the cursor is, or lock to a screen coordinate you pick visually
- ⌨️ **Global hotkey toggle** — start/stop clicking from any window with a customizable hotkey (default `F6`)
- 🧰 **System tray support** — minimize to tray or taskbar, with your preference remembered
- ⚙️ **Persistent settings** — all click parameters and preferences are saved between sessions
- 🔄 **Built-in auto-update** — WinSparkle on Windows, a GitHub Releases–based flow on macOS/Linux
- 🛑 **Remote version kill switch** — a shipped build with a known issue can be remotely retired; affected running copies are notified and shut down gracefully instead of silently continuing
- 🧪 **Tested core** — click engine, config persistence, single-instance guard, and updater logic are covered by an automated test suite
- 🚀 **One-command CI builds** — GitHub Actions builds signed Windows/macOS/Linux binaries on every push and publishes them on tagged releases

## Showcase

> Auto Clicker in a few numbers and highlights:

| | |
|---|---|
| 🖥️ **Cross-platform** | Single codebase, native builds for Windows, macOS, and Linux |
| ⚡ **Sub-millisecond accuracy** | Sleep-then-spin timing loop keeps click intervals tight even at high frequency |
| 🪶 **Lightweight** | No background services beyond the app itself — starts, clicks, and gets out of the way |
| 🔐 **Signed releases** | Windows/macOS builds and update feeds are cryptographically signed |
| 🤖 **CI-built binaries** | Every release is built and published automatically via GitHub Actions |

*(Add screenshots or a short GIF of the app here once available — a picture of the click-settings panel and tray icon in action goes a long way for new visitors.)*

## Release & Support Lifecycle

| Version | Status | Platforms | Notes | Support Ends |
|---------|--------|-----------|-------|---------------|
| 1.0.0   | ✅ Current | Windows, macOS, Linux | Initial public release | — |
| —       | 🔜 Planned | — | Fill in as new versions ship | — |

**Legend:** ✅ Current • 🔧 Maintenance (critical fixes only) • 🚫 End of life (no longer supported)

> A version can be remotely retired via the app's built-in kill switch if it ships with a serious bug (e.g. a broken updater). Affected installs are notified on their next check-in and prompted to update.

## Getting Started

### Requirements

- Python **3.10+**
- Dependencies listed in [`requirements.txt`](requirements.txt) (PyQt6, pynput)

### Run from source

```bash
# Clone the repository
git clone https://github.com/ToshiroSky/auto-clicker.git
cd auto-clicker

# (Recommended) create a virtual environment
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch the app
python auto_clicker_app.py
```

### Platform-specific notes

- **macOS** — the app (or your terminal/Python interpreter, if running from source) needs **Accessibility** permission under *System Settings → Privacy & Security → Accessibility* for clicks to register.
- **Linux (Wayland)** — works out of the box under X11/XWayland. On a pure-Wayland session without XWayland, you may need the `uinput` backend and access to `/dev/uinput` (add your user to the `input` group or set up the appropriate udev rule).
- **Chrome OS** — the Linux (Crostini) container behaves like a regular Linux install; the same X11/XTest path applies.

### Running tests

```bash
pip install -r requirements-dev.txt
pytest
```

### Building a standalone binary

Binaries are built with PyInstaller; see [`.github/workflows/build.yml`](.github/workflows/build.yml) for the exact build/sign/release pipeline used for official releases.

## Usage

1. Launch the app.
2. Set your desired interval, mouse button, click type, and repeat mode.
3. Choose **current position** or pick a **fixed position** on screen.
4. Press **Start** (or your configured hotkey — default `F6`) to begin clicking, and press it again to stop.
5. Minimize to the tray or taskbar to keep it running in the background.

## Contributing

Issues and pull requests are welcome. If you're proposing a larger change, please open an issue first to discuss what you'd like to change.

## License

*(No license file is currently included in this repository — add a `LICENSE` file and update this section before distributing binaries or accepting external contributions.)*

## Disclaimer

Auto-clicking may violate the terms of service of some games, applications, or platforms. Use responsibly and at your own risk.
