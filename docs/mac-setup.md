---
layout: default
title: Setup for macOS
---

# 🍏 macOS Development Setup Guide

Set up your development environment for .NET MAUI on macOS using Visual Studio Code.

---

## ✅ Requirements

- **macOS Monterey or newer**
- [Visual Studio Code](https://code.visualstudio.com/)
- [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download)
- [Java Development Kit (JDK 17+)](https://adoptium.net/)
- [Android Studio](https://developer.android.com/studio)
- [Homebrew](https://brew.sh/)

---

## 1️⃣ Install Prerequisites

### Install Homebrew (if not already installed)

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

---

### Install .NET SDK

```bash
brew install --cask dotnet-sdk
```

Or download directly from [.NET Downloads](https://dotnet.microsoft.com/en-us/download).

---

### Install JDK

```bash
brew install --cask temurin
```

Verify:

```bash
java -version
```

---

### Install Android Studio

1. Install with Homebrew:

   ```bash
   brew install --cask android-studio
   ```

2. Open Android Studio → Complete initial setup

3. Go to **Device Manager** → Create an Android Virtual Device (AVD)

---

## 2️⃣ Install .NET MAUI Workload

```bash
dotnet workload install maui
```

---

## 3️⃣ Clone the Repository

```bash
git clone https://github.com/your-org/your-repo.git
cd your-repo
```

---

## 4️⃣ Build & Run

```bash
dotnet build
dotnet run
```

To target Android explicitly:

```bash
dotnet run -f:net8.0-android
```

---

## 5️⃣ Open in VS Code

```bash
code .
```

### Recommended Extensions:

- C# Dev Kit
- MAUI Toolkit
- XML Tools
- Android Emulator

---

## ✅ Done!

You're all set up to build and run the MAUI app on macOS.
