# Quick Notes 📝⚡

> **A production-grade, ultra-fast, 100% offline dark-mode to-do app for Android.**  
> Inspired by the sleek minimalism of Apple Notes and Google Pixel Material You.

[![Android](https://img.shields.io/badge/Platform-Android_8.0+_(API_26+)-3DDC84?logo=android&logoColor=white)](#)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](#)
[![Theme](https://img.shields.io/badge/Theme-Dark_Mode_Only-000000?logo=github)](#)
[![Privacy](https://img.shields.io/badge/Network-0%25_Offline_(No_Internet)-success)](#)
[![Size](https://img.shields.io/badge/APK_Size-1.88_MB-informational)](#)

---

## 📥 Download

Get the official signed release APK directly:

- 📦 **[Download QuickNotes-1.0.apk](QuickNotes-1.0.apk)** *(1.88 MB)*

### Verification (SHA-256)
```text
884A715CD5B33361E773AE50DA70DB47BCED85258984B2A67A33E1DA0882E0C7
```
To verify the integrity on your computer:
```powershell
Get-FileHash QuickNotes-1.0.apk -Algorithm SHA256
```
Or on macOS / Linux:
```bash
sha256sum QuickNotes-1.0.apk
```

---

## ✨ Features

- **⚡ Instant Launch:** Opens directly into your task list with zero splash screen delays, zero spinners, and zero sync wait times.
- **🌙 True OLED Pitch Black:** Built exclusively for dark mode with pure `#000000` background, subtle surface elevations, and warm amber accents. No blinding light themes.
- **📝 Dual Note Modes:**
  - **Simple Mode:** Fast, flexible checkbox notes for quick thoughts and to-dos.
  - **Advanced Mode:** Single-line bold title with an expandable detail body for complex tasks.
- **👆 Fluid Gestures:**
  - Swipe right on any task to instantly mark it complete.
  - Interactive confetti burst when finishing your tasks.
  - Collapsed **Completed** archive keeps your workspace clean and decluttered.
- **⏰ Smart Offline Reminders:**
  - One-tap quick presets: *"Today 6:00 PM"*, *"Tomorrow 8:00 AM"*, or custom date & time picker.
  - Rich notifications with interactive quick action buttons (**Mark Complete** or **Snooze 15 Min** right from the notification drawer).
  - Reliable boot recovery (`RECEIVE_BOOT_COMPLETED`) restores pending reminders if your phone restarts.
- **📱 1×1 Home Screen Quick Widget:** Tap the home screen widget to jump straight into note creation with the keyboard ready.
- **🔒 Privacy by Architecture:**
  - **Zero internet permission:** The `android.permission.INTERNET` permission is completely omitted from the app manifest. Your notes physically cannot leave your phone.
  - **App-Private Local Storage:** Backed by encrypted local Room/SQLite database with cloud backup extraction disabled.
  - **Zero telemetry, zero analytics, zero ads.**

---

## 📲 How to Install

1. Download **`QuickNotes-1.0.apk`** onto your Android phone (Android 8.0 Oreo or newer).
2. Tap the downloaded file in your browser or file manager.
3. If prompted, allow **"Install unknown apps"** for your browser or file manager.
4. Tap **Install** and open **Quick Notes**!

---

## 🛠️ Architecture & Tech Stack

- **Language:** Kotlin 1.9+
- **UI Toolkit:** Jetpack Compose (Material 3 foundation, customized pure dark design system)
- **Architecture:** Single-Activity, ViewModel + Flow + StateFlow
- **Database:** AndroidX Room with KSP
- **Alarms:** Exact alarm scheduling (`AlarmManager` + `BroadcastReceiver`)
- **Optimization:** ProGuard / R8 code and resource shrinking (compiled to under 2 MB)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
