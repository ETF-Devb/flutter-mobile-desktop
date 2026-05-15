<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=soft&color=9D50BB&height=240&section=header&text=ETF-Devb&fontSize=80&animation=fadeIn&desc=LINUX+DEVELOPMENT+ON+ANDROID&descSize=20&descAlignY=65" width="100%" />
</p>

<p align="center">
  <img width="220" src="https://github.com/user-attachments/assets/2402e001-631b-49fa-9c4e-bf63a92591ed" style="border-radius: 50%; border: 4px solid #9D50BB; box-shadow: 0 0 30px #9D50BB;" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Orbitron&weight=700&size=32&pause=1000&color=9D50BB&center=true&vCenter=true&width=700&lines=🚀+FLUTTER+LINUX+ON+ANDROID+READY;🛠️+UDROID+JAMMY+CORE+LOADED;🖥️+DESKTOP+INTERFACE+ACTIVE" alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/Termux-000000?style=for-the-badge&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Ubuntu-E94333?style=for-the-badge&logo=ubuntu&logoColor=white" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=ETF-Devb&label=VISITOR%20COUNT&color=9D50BB&style=flat-square" />
</p>

---

## 💎 <font color="#9D50BB">Desktop Preview</font>
<p align="center">
  <div style="border: 2px solid #9D50BB; border-radius: 20px; padding: 12px; background: #0d1117; box-shadow: 0 0 40px rgba(157, 80, 187, 0.3);">
    <img src="https://github.com/user-attachments/assets/418d1858-54ee-4ccb-9feb-fcee40327081" width="100%" style="border-radius: 12px;" alt="Workstation Environment" />
  </div>
</p>

---

## 📥 <font color="#9D50BB">Required Apps</font>

| App Name | Download Link | Status |
| :--- | :--- | :--- |
| **Termux App** | [![Download](https://img.shields.io/badge/V1.0.0_APK-Black?style=for-the-badge&logo=github)](https://github.com/ETF-Devb/Mobile-Workstation-Pro/releases/tag/v1.0.0) | `SECURE` |
| **Termux-X11** | [![Download](https://img.shields.io/badge/V1.0.0_APK-Black?style=for-the-badge&logo=github)](https://github.com/ETF-Devb/Mobile-Workstation-Pro/releases/tag/v1.0.0) | `STABLE` |

---

## 🏁 <font color="#9D50BB">How to Start</font>

### 🛸 PART 1: Launch the Screen

**Step 1: Start X11 Engine**
```bash
termux-x11 :1 -ac &

```

> [!IMPORTANT]
> Switch to the **Termux-X11 App** and keep it running in the background.

**Step 2: Log into Ubuntu**

```bash
udroid login jammy:xfce4

```

**Step 3: Open Desktop**

```bash
export DISPLAY=:1 && service dbus start && startxfce4 &

```

---

### 🐧 PART 2: Setup Coding Tools

*Open the Terminal inside your new Desktop screen to run these commands.*

**Step 4: Update System**

```bash
apt update

```

**Step 5: Install Requirements**

```bash
apt install -y curl git unzip xz-utils zip libglu1-mesa clang cmake ninja-build pkg-config libgtk-3-dev liblzma-dev libstdc++-12-dev

```

**Step 6: Download Flutter**

```bash
cd ~ && git clone https://github.com/flutter/flutter.git -b stable

```

**Step 7: Set Path**

```bash
echo 'export PATH="$PATH:$HOME/flutter/bin"' >> ~/.bashrc

```

**Step 8: Save Changes**

```bash
source ~/.bashrc

```

---

### 🚀 PART 3: Run Your App

**Step 9: Create Project**

```bash
flutter create etf_devb_app

```

**Step 10: Go to Folder**

```bash
cd etf_devb_app

```

**Step 11: Launch App**

```bash
flutter run -d linux

```
