<p align="center">
  <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/purple.png" width="100%">
</p>

<h1 align="center">
  <font color="#9D50BB">⚡ FLUTTER LINUX DESKTOP ON ANDROID ⚡</font>
</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" />
  <img src="https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/Ubuntu-E94333?style=for-the-badge&logo=ubuntu&logoColor=white" />
  <img src="https://img.shields.io/badge/Termux-000000?style=for-the-badge&logo=linux&logoColor=white" />
</p>

<p align="center">
  https://github.com/user-attachments/assets/e7ad0058-8768-4ad9-819e-8d5b21dddbec
</p>

---

## 🛠️ Prerequisites

| Module | Source | Status |
| :--- | :--- | :--- |
| **Termux** | F-Droid Version | `REQUIRED` |
| **Termux-X11** | GitHub Releases | `REQUIRED` |
| **Udroid** | Ubuntu Jammy Environment | `READY` |

---

## 🏁 PHASE 1: SYSTEM INITIALIZATION

### 🟢 STEP 1: DEPLOY DISPLAY SERVER
```bash
termux-x11 :1 -ac &

```

### 🟢 STEP 2: UBUNTU CORE LOGIN

```bash
udroid login jammy:xfce4

```

---

## 🐧 PHASE 2: DEPENDENCY INJECTION

### 🔵 STEP 3: INSTALL LINUX TOOLCHAIN

```bash
apt update && apt install -y curl git unzip xz-utils zip libglu1-mesa \
clang cmake ninja-build pkg-config libgtk-3-dev liblzma-dev libstdc++-12-dev

```

### 🔵 STEP 4: FLUTTER SDK CLONING

```bash
cd ~
git clone [https://github.com/flutter/flutter.git](https://github.com/flutter/flutter.git) -b stable

```

### 🔵 STEP 5: PATH CONFIGURATION

```bash
echo 'export PATH="$PATH:$HOME/flutter/bin"' >> ~/.bashrc
source ~/.bashrc

```

---

## 🖥️ PHASE 3: THE INCEPTION

### 🟣 STEP 6: LAUNCH GUI (XFCE4)

```bash
export DISPLAY=:1 && service dbus start && startxfce4 &

```

### 🟣 STEP 7: PROJECT SCAFFOLDING

```bash
flutter create my_viral_app
cd my_viral_app

```

### 🟣 STEP 8: THE FINAL KICK

```bash
flutter run -d linux

```

---
