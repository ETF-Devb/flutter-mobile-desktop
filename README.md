## 🛠 Prerequisites

Ensure you have these installed:

* **Termux** (F-Droid version)
* **Termux-X11** app
* **Udroid** environment (Ubuntu Jammy)

---

## 🏁 Phase 1: Termux Initial Setup (The "Black Screen" Phase)

### 0️⃣ Step 0: Clean Start

> [!IMPORTANT]
> First, close all existing sessions and open a **fresh/clean** Termux terminal to avoid any background conflicts.

### 1️⃣ Step 1: Start X11 Display Server

Run the following command to initialize the display server:

```bash
termux-x11 :1 -ac &

```

> **Action Required:** Now, exit Termux (keep it running in the background) and **open the Termux-X11 app**. Leave it active in the background.

### 2️⃣ Step 2: Enter Ubuntu Environment

Login to your Udroid environment (No need to type "termux" at the start):

```bash
udroid login jammy:xfce4

```

*Wait until you see `root@localhost:~#`—this confirms you are inside.*

---

## 🐧 Phase 2: Ubuntu Preparation & Flutter Setup

### 3️⃣ Step 3: Install Required Linux Libraries

Copy and paste this one-liner to install all Flutter dependencies for Linux:

```bash
apt update && apt install -y curl git unzip xz-utils zip libglu1-mesa \
clang cmake ninja-build pkg-config libgtk-3-dev liblzma-dev libstdc++-12-dev

```

### 4️⃣ Step 4: Download Flutter SDK

Clone the stable branch into your home directory:

```bash
cd ~
git clone https://github.com/flutter/flutter.git -b stable

```

### 5️⃣ Step 5: Define Flutter in PATH

Make the `flutter` command accessible globally:

```bash
echo 'export PATH="$PATH:$HOME/flutter/bin"' >> ~/.bashrc
source ~/.bashrc

```

---

## 🖥️ Phase 3: Launch & Execute (The "Inception")

### 6️⃣ Step 6: Start Graphical Interface (XFCE)

Run this command to bring up the desktop (Copy-paste as one line):

```bash
export DISPLAY=:1 && service dbus start && startxfce4 &

```

> **Note:** Now check your **Termux-X11 app**; the Ubuntu desktop should be visible.

### 7️⃣ Step 7: Create Your First Project

Open the **Terminal** inside XFCE and run:

```bash
flutter create my_viral_app
cd my_viral_app

```

### 8️⃣ Step 8: The "Final Kick" - Run the App

Launch your app as a native Linux Desktop application:

```bash
flutter run -d linux

```
