
<p align="center">
  <img width="280" src="https://github.com/user-attachments/assets/2402e001-631b-49fa-9c4e-bf63a92591ed" style="border-radius: 20px; filter: drop-shadow(0 0 10px #9D50BB);" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=700&size=35&pause=1000&color=9D50BB&center=true&vCenter=true&width=600&lines=⚡+FLUTTER+LINUX+DESKTOP+⚡;⚡+RUNNING+ON+ANDROID+⚡;⚡+ULTIMATE+WORKSTATION+⚡" alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" />
  <img src="https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/Ubuntu-E94333?style=for-the-badge&logo=ubuntu&logoColor=white" />
  <img src="https://img.shields.io/badge/Termux-000000?style=for-the-badge&logo=linux&logoColor=white" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=9D50BB&height=60&section=header" width="100%" />
</p>

<p align="center">
  <b>The ultimate workstation setup for mobile-based Linux development.</b>
  <br />
  <i>Optimized for performance, styled for professionals.</i>
</p>

<p align="center">
  <table align="center">
    <tr>
      <td align="center" style="border: 2px solid #9D50BB; border-radius: 20px; background-color: #0d1117;">
        <br>
        <img src="https://github.com/user-attachments/assets/418d1858-54ee-4ccb-9feb-fcee40327081" width="100%" style="border-radius: 15px;" />
        <br>
        <img src="https://img.shields.io/badge/SYSTEM-ACTIVE-brightgreen?style=for-the-badge" />
        <br><br>
      </td>
    </tr>
  </table>
</p>

---

## 🛠️ <font color="#9D50BB">Core Modules</font>

| Module | Deployment Source | Status |
| :--- | :--- | :--- |
| **Termux** | [![Download](https://img.shields.io/badge/Download_APK-Black?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ETF-Devb/Mobile-Workstation-Pro/releases/tag/v1.0.0) | `REQUIRED` |
| **Termux-X11** | [![Download](https://img.shields.io/badge/Download_APK-Black?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ETF-Devb/Mobile-Workstation-Pro/releases/tag/v1.0.0) | `REQUIRED` |
| **Udroid** | [Ubuntu Jammy Environment] | `READY` |

---

## 🏁 <font color="#9D50BB">PHASE 1: SYSTEM INITIALIZATION</font>

### 🟢 STEP 1: DEPLOY DISPLAY SERVER
```bash
termux-x11 :1 -ac &

```

> [!IMPORTANT]
> Switch to the **Termux-X11 App** immediately and keep it active in the background.

### 🟢 STEP 2: UBUNTU CORE LOGIN

```bash
udroid login jammy:xfce4

```

---

## 🐧 PHASE 2: DEPENDENCY INJECTION

### 🔵 STEP 3: INSTALL TOOLCHAIN

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

### 🟣 STEP 7: RUN PROJECT

```bash
flutter create my_viral_app && cd my_viral_app
flutter run -d linux

```
