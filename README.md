# 🐾 rp2040-dev - BitDogLab Edition ((🚧Work in progress))

A complete and professional Docker environment for developing with the **Raspberry Pi Pico (RP2040)** — carefully crafted and maintained by **alfecjo for BitDogLab**.

---

## ✅ What's Included

Everything you need to get started with RP2040 development using **Visual Studio Code Dev Containers**:

- 🛠️ Raspberry Pi Pico SDK
- 💡 Official `pico-examples` pre-cloned
- 📦 `gcc-arm-none-eabi` toolchain (v10.3)
- 🔧 Precompiled `picotool`
- ✅ CMake + Ninja + GDB (multiarch)
- 🐍 Python 3 with `pip`, `setuptools`, and useful packages
- 🐧 Ubuntu 24.04 base image
- 👤 Pre-configured `dev` user with correct permissions
- 🧠 Automatic support for `.vscode` folder inside the examples

---

## 💡 Fully Optimized for Dev Containers

- 👤 This image is built **exclusively** for use with [Dev Containers](https://code.visualstudio.com/docs/devcontainers/containers), providing a **professional, reproducible, and portable** development setup.

---

## 🚀 How to Use

### 1. Requirements

- [Docker](https://www.docker.com/)
- [Visual Studio Code](https://code.visualstudio.com/)
- Extension: **Dev Containers** (by Microsoft)

---

### 2. Using the Dev Container

- 🧠 Use this image inside your `.devcontainer/devcontainer.json` like so:

```json
{
  "name": "RP2040 Dev",
  "image": "alfecjo/rp2040-dev:latest",
  "features": {},
  "remoteUser": "dev"
}
```

---

### 3. Pull the Docker Image

```C
docker pull alfecjo/rp2040-dev:latest
```

---

### 4. View available tags:

🔗 [Docker Hub](https://hub.docker.com/r/alfecjo/rp2040-dev/tags)

---

## 🎯 Optional: Run and Connect Manually via Docker CLI

- If you prefer not to use Dev Containers, you can still use this image by launching the container manually and connecting to it from Visual Studio Code.

### 🔄 1. Run the Container

- Start a new container from the image:

```bash
docker run -it --name rp2040-dev-container --rm \
  -v ${PWD}:/workspace \
  alfecjo/rp2040-dev:latest \
  bash
```

## 🔧 This command will:

- 1. Run the container interactively
- 2. Mount the current directory (${PWD}) to /workspace inside the container
- 3. Use the dev user
- 4. Automatically remove the container after exiting

🔗 If you want to keep the container running in the background, omit --rm and use -d instead:

```bash

  docker run -dit --name rp2040-dev-container \
  -v ${PWD}:/workspace \
  alfecjo/rp2040-dev:latest

```

### 💻 2. Connect from VS Code

- In a local terminal (outside the container), run:

```bash

code --remote "containers://rp2040-dev-container"

```

- his opens the running container directly in VS Code!

**Make sure you have the Remote - Containers extension installed.**

### 🛠️ 3. Stop the Container (if not using --rm)

- When done, you can stop and remove the container:

```bash

docker stop rp2040-dev-container
docker rm rp2040-dev-container

```