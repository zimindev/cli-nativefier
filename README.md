# 🎯 Nativefier — Create Desktop Apps from Websites

**Nativefier** is a command-line tool that lets you quickly create a native desktop application for any website using Electron. It wraps any web page into a cross-platform desktop app for Windows, macOS, or Linux.

---

## ✅ Features

* Turn any website into a standalone desktop app
* Cross-platform support: Windows, macOS, Linux
* Customize app name, icon, user agent, and more
* Supports fullscreen, kiosk mode, system tray, and custom CSS/JS injection
* No coding required — just one command to build your app

---

## 📦 Installation

### Prerequisite: Install Node.js and npm

Make sure you have **Node.js** (version 12 or later) and **npm** installed on your system.

---

### Ubuntu / Debian

```bash
sudo apt update
sudo apt install nodejs npm
```

*If the default Node.js version is old, you can install a newer version from NodeSource:*

```bash
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs
```

Then install Nativefier globally:

```bash
sudo npm install -g nativefier
```

---

### Fedora

```bash
sudo dnf install nodejs npm
sudo npm install -g nativefier
```

---

### Arch Linux

```bash
sudo pacman -S nodejs npm
sudo npm install -g nativefier
```

---

## 🚀 Basic Usage

### Create a desktop app for a website

```bash
nativefier "https://example.com"
```

### Example: Make WhatsApp Desktop app with custom icon

```bash
nativefier --name "WhatsApp" --icon whatsapp.ico "https://web.whatsapp.com"
```

---

## ⚙️ Options & Examples

| Option                     | Description                            |                  |                             |
| -------------------------- | -------------------------------------- | ---------------- | --------------------------- |
| `--name "AppName"`         | Set the desktop app name               |                  |                             |
| `--icon /path/to/icon`     | Use a custom icon (.ico, .icns, .png)  |                  |                             |
| \`--platform \[windows     | mac                                    | linux]\`         | Target platform for the app |
| \`--arch \[x64             | arm64]\`                               | CPU architecture |                             |
| `--user-agent "UA string"` | Override browser user agent            |                  |                             |
| `--fullscreen`             | Launch app in fullscreen mode          |                  |                             |
| `--kiosk`                  | Enable kiosk mode (no window controls) |                  |                             |
| `--inject /path/to/file`   | Inject custom CSS or JavaScript        |                  |                             |

---

## 🧩 Tips

* Use custom icons for professional look
* Disable dev tools for security with `--disable-dev-tools`
* Combine with system tray support for background apps
* Great for turning web tools, chats, or dashboards into desktop apps

---

## 📚 More Info

* GitHub: [https://github.com/nativefier/nativefier](https://github.com/nativefier/nativefier)
* Docs: See README on GitHub for full usage and advanced options
