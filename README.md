# My Custom KDE Plasma Dotfiles 🍵

This repository contains a backup of the layout configurations, interface settings, and design assets for my personalized desktop environment. It sets up a streamlined, minimal bottom panel dock matched with a dark jade/mint color profile, frosted glass windows, and snappy application layouts.

---

## 💻 My Machine & OS Baseline

These configuration choices map directly to the hardware acceleration paths and system layers of my laptop:

* **OS / Desktop:** Fedora Linux 44 running native KDE Plasma (Wayland)
* **Linux Kernel:** `7.2.7-200.fc44.x86_64`
* **KDE Plasma Version:** 6.7.5
* **KDE Frameworks Version:** 6.30.0
* **Qt Version:** 6.11.2
* **Core Fonts Used:** GoogleSansCode Nerd Font & JetBrains Mono

---

## 📂 Repository File Inventory

* **`kdeglobals`** – Universal system parameters handling interface typography, font sizes, and active colors.
* **`kwinrc`** – Window manager engine layout rules governing wobbly window speeds, automatic 3-column tiling, and Better Blur DX frosted transparency balances.
* **`breezerc`** – Core application styling definitions, including the explicit 20% menu opacity setting (`MenuOpacity=80`) and deep window contrast drop shadow depths.
* **`plasma-org.kde.plasma.desktop-appletsrc`** – Structural layout geometry coordinates that shrink and center the bottom panel into a clean application dock.
* **`color-schemes/`** – A directory containing 12 custom color palette files, including the primary dark forest green `OmarchyShadesOfJade` theme.
* **`wallpapers.zip`** – A standalone asset archive containing my collection of dark jade/mint themed desktop backgrounds, curated directly from the Omarchy Theme ecosystem.

---

## 🔄 File Placement & Theme Component Reference

To manually restore this exact look on a fresh installation of Fedora KDE, make sure you turn off your desktop shell first (run `kquitapp6 plasmashell` in a terminal so system components don't overwrite your changes). 

Then, simply place the repository configuration assets into their respective system locations and download the core external packages from their original project hubs:

### 1. Main System Configurations
Paste the core configuration files straight into your hidden user settings folder:
* **Target Directory:** `~/.config/`
* **Files to Place Here:** `kdeglobals`, `kwinrc`, `breezerc`, and `plasma-org.kde.plasma.desktop-appletsrc`

### 2. Custom Color Palettes
Paste the entire folder containing your custom `.colors` profiles here:
* **Target Directory:** `~/.local/share/color-schemes/`
* **What to Place Here:** The whole `color-schemes` directory and its contents.


### 📦 Mandatory Visual Components (External Projects)
The core theme components below are excluded from this repository and must be pulled directly from their official open-source project channels:

* **Desktop Icons & Cursors Engine:** Install the baseline layout assets straight via the official [Papirus Development Team's Icon Repository](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme).
* **The Login Screen Interface Theme:** Get the **Forest** login screen style environment explicitly out of the [Darkkal44 Qylock GitHub Repository](https://github.com/Darkkal44/qylock).
* **Window Blur Engine:** Install the **Better Blur DX** plugin through the KDE System Settings (under Window Management ➔ KWin Scripts) so the system can read the custom transparency rules stored in `kwinrc`.
* **System Typography:** Download and install the **GoogleSansCode Nerd Font** package (both `Mono` and `Propo` variations) alongside the **JetBrains Mono** font family. Without these installed locally, interface text and panel applet dimensions will default to stock text configurations and break alignment.


Once your files are dropped cleanly into place and your external theme packages are installed, turn your graphical interface backend engine back on (run `kstart6 plasmashell` in a terminal) to load the workspace!

---

