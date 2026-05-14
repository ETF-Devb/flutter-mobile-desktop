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
  <b>The ultimate workstation setup for mobile-based Linux development.</b>
  <br />
  <i>Optimized for performance, styled for professionals.</i>
</p>

---

## 🛠️ Prerequisites

Before initiating the sequence, ensure the following core modules are active:

| Module | Source | Status |
| :--- | :--- | :--- |
| **Termux** | F-Droid Version | `REQUIRED` |
| **Termux-X11** | GitHub Releases | `REQUIRED` |
| **Udroid** | Ubuntu Jammy Environment | `READY` |

---

## 🏁 PHASE 1: SYSTEM INITIALIZATION
> *The "Black Screen" Protocol*

### 🟢 STEP 0: ENVIRONMENT PURGE
Close all active sessions. Open a **Clean Terminal** to prevent kernel-level conflicts.

### 🟢 STEP 1: DEPLOY DISPLAY SERVER
Initialize the X11 backend:
```bash
termux-x11 :1 -ac &

```

> [!IMPORTANT]
> Switch to the **Termux-X11 App** immediately and keep it active in the background.

### 🟢 STEP 2: UBUNTU CORE LOGIN

Access the Udroid environment (Jammy/XFCE4):

```bash
udroid login jammy:xfce4

```

*Wait for the `root@localhost:~#` prompt before proceeding.*

---

## 🐧 PHASE 2: DEPENDENCY INJECTION

> *Building the Development Core*

### 🔵 STEP 3: INSTALL LINUX TOOLCHAIN

Copy and paste this high-speed installation string:

```bash
apt update && apt install -y curl git unzip xz-utils zip libglu1-mesa \
clang cmake ninja-build pkg-config libgtk-3-dev liblzma-dev libstdc++-12-dev

```

### 🔵 STEP 4: FLUTTER SDK CLONING

Inject the stable Flutter branch into your home directory:

```bash
cd ~
git clone [https://github.com/flutter/flutter.git](https://github.com/flutter/flutter.git) -b stable

```

### 🔵 STEP 5: PATH CONFIGURATION

Register Flutter globally in the system bash environment:

```bash
echo 'export PATH="$PATH:$HOME/flutter/bin"' >> ~/.bashrc
source ~/.bashrc

```

---

## 🖥️ PHASE 3: THE INCEPTION

> *Executing Graphical Desktop & Project Build*

### 🟣 STEP 6: LAUNCH GUI (XFCE4)

Activate the desktop environment and DBUS services:

```bash
export DISPLAY=:1 && service dbus start && startxfce4 &

```

*Your mobile screen is now a fully functional Linux PC.*

### 🟣 STEP 7: PROJECT SCAFFOLDING

Initialize your first "Viral" application:

```bash
flutter create my_viral_app
cd my_viral_app

```

### 🟣 STEP 8: THE FINAL KICK

Run your application as a native Linux desktop entity:

```bash
flutter run -d linux

```

---


5. **Neon Lines:** زدت خطوط بنفسجية (Purple Lines) في البداية والنهاية باش تعطي داك الستيل ديال "Neon Glow".

هاد الملف دابا تقدر تحطو في GitHub ديالك وأنت مرتاح، كيبان ديال "عشاق الكود" الحقيقيين! واش ناضي هكا؟
