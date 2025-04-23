# 🐾 rp2040-dev – BitDogLab Edition

A complete and professional Docker-based development environment for the **Raspberry Pi Pico (RP2040)** — curated and maintained by [alfecjo](https://github.com/alfecjo) for **BitDogLab**.

---

## ✅ What's Included

Everything you need for RP2040 firmware development using **Visual Studio Code Dev Containers**:

- 🛠️ Raspberry Pi Pico SDK (with `pico-examples`)
- 📦 `gcc-arm-none-eabi` toolchain v10.3
- 🔧 Precompiled `picotool`
- ⚙️ CMake, Ninja, and multiarch GDB
- 🐍 Python 3 + `pip`, `setuptools`, and dev packages
- 🧠 Auto-mount `.vscode` settings to examples
- 🐧 Ubuntu 24.04 base
- 👤 Preconfigured `dev` user with proper permissions

---

## 💡 Why Dev Containers?

This image is **purpose-built for Dev Containers**, giving you:

- 🧪 Reproducible builds
- 🚀 Rapid onboarding
- 🧳 Fully portable environments
- 💻 Consistent toolchains across teams and OSes

---

## 🚀 Quick Start Guide

### ✅ Requirements

| Tool            | Link                                  |
|-----------------|---------------------------------------|
| Docker DeskTop  | https://www.docker.com/               |
| VS Code         | https://code.visualstudio.com/        |
| Dev Containers  | Extension by Microsoft                |

![Docker: Install](img/img004.jpg)
![VSC: Install](img/img005.jpg)
![Dev Containers: Install](img/img004.jpg)

---

### 🔧 Cloning and Launching

```bash
git clone https://github.com/alfecjo/rp2040-container.git
cd rp2040-dev
code .
```

### 📁 When prompted by VS Code, click "Reopen in Container".

![Dev Containers: Reopen Containers](img/img001.jpg)

![Dev Containers: Reopen Containers](img/img002.jpg)

![Dev Containers: Reopen Containers](img/img003.jpg)



