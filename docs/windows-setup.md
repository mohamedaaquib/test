---
layout: default
title: Setup for Windows
---

# 🪟 Windows Development Setup Guide

This guide will walk you through setting up a development environment for .NET MAUI using **Visual Studio Code** on Windows.

---

## ✅ Requirements

- **Windows 10/11 (64-bit)**
- [Visual Studio Code](https://code.visualstudio.com/)
- [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download)
- [Java Development Kit (JDK 17+)](https://adoptium.net/)
- [Android Studio](https://developer.android.com/studio)
- Git

---

## 1️⃣ Install Required Tools

### .NET 8 SDK

```bash
winget install Microsoft.DotNet.SDK.8
```

Or [download manually](https://dotnet.microsoft.com/en-us/download/dotnet/8.0).

---

### Java (JDK 17+)

```bash
winget install Eclipse.Temurin.17.JDK
```

Confirm installation:

```bash
java -version
```

---

### Android Studio

1. Download from [developer.android.com](https://developer.android.com/studio)
2. During install, make sure the **Android SDK**, **AVD Manager**, and **Emulator** are selected.
3. After installation:
   - Open **Device Manager**
   - Create a Virtual Device (e.g. Pixel 5, API 34)
   - Launch emulator

---

## 2️⃣ Install .NET MAUI Workloads

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

## 4️⃣ Run the App

```bash
dotnet build
dotnet run
```

---

## 5️⃣ Open in VS Code

```bash
code .
```

### Recommended Extensions:

- C# Dev Kit
- .NET MAUI (if available)
- Android Emulator
- XML Tools

---

## 🧪 Test on Emulator

1. Start your Android Emulator via Android Studio or AVD Manager
2. Run the app again:
   ```bash
   dotnet run -f:net8.0-android
   ```

---

## 🎉 You're Ready!

You now have a full development setup for .NET MAUI on Windows using VS Code.
