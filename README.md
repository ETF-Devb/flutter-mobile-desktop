
<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.x-02569B?style=for-the-badge&logo=flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/Dart-SDK-0175C2?style=for-the-badge&logo=dart&logoColor=white" />
  <img src="https://img.shields.io/badge/Environment-Ubuntu_Jammy-E95420?style=for-the-badge&logo=ubuntu&logoColor=white" />
  <img src="https://img.shields.io/badge/IDE-VS_Code_OSS-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" />
</p>

<p align="center">
  <img src="https://images2.imgbox.com/71/9b/7pI6kYfC_o.png" width="850" alt="Flutter on Android Preview" />
</p>

---

### [ >_ DEVELOPMENT_SUITE ]
> **Project:** Mobile Flutter Dev-Station  
> **Target:** Build & Run Cross-Platform Apps directly from Android (via Udroid).

<a href="https://github.com/ETF-Devb/Mobile-Workstation-Pro/releases">
  <img src="https://img.shields.io/github/v/release/ETF-Devb/Mobile-Workstation-Pro?style=for-the-badge&color=02569B&label=DOWNLOAD%20DEV%20ASSETS&logo=github" />
</a>

---

### [ >_ FLUTTER_INSTALLATION_FLOW ]

#### 1. System Preparation
Before installing Flutter, we must ensure all native dependencies are present in our Ubuntu environment.
```bash
# Update repositories and install essential build tools
sudo apt update && sudo apt upgrade -y
sudo apt install git curl unzip xz-utils zip libglu1-mesa clang cmake ninja-build pkg-config libgtk-3-dev -y

```

#### 2. Fetching Flutter SDK

We will use the stable branch to ensure maximum reliability on mobile-proot environments.

```bash
# Clone Flutter directly to your home directory
git clone [https://github.com/flutter/flutter.git](https://github.com/flutter/flutter.git) -b stable

```

#### 3. Path Configuration

To execute `flutter` commands from anywhere, we need to export the binary path.

```bash
# Add Flutter to your environment path
export PATH="$PATH:`pwd`/flutter/bin"

# Verify installation (This will download Dart SDK automatically)
flutter doctor

```

---

### [ !_ WORKSPACE_INITIALIZATION ]

#### Step 1: Create Your First Project

Initialize a clean Flutter boilerplate project.

```bash
flutter create my_first_app
cd my_first_app

```

#### Step 2: Launching the Editor

We recommend using **VS Code (OSS)** for a lightweight yet powerful experience.

```bash
# Open your project in the editor
code .

```

#### Step 3: Execution Protocol (Linux Desktop Mode)

Since we are running inside XFCE4, we will run the app as a **Linux Desktop App** for testing.

```bash
# Run the application in debug mode
flutter run -d linux

```

---

### [ X_ CLEANUP_PROTOCOL ]

If you encounter "Lock" issues or want to clear the build cache:

```bash
# Clear build artifacts
flutter clean

# Kill any hanging dart processes
pkill -9 dart

```

---

---
