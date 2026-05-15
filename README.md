# Namma-Raste Reporter

Native Android Kotlin app for rapid infrastructure reporting. Citizens can capture a pothole or broken streetlight photo, attach automatic time and GPS metadata, generate a unique ticket ID, and track locally saved reports.

## Features

- Simple citizen login to reduce spam.
- CameraX live preview and photo capture.
- Issue type selection for potholes and streetlights.
- Severity selection for low, medium, and high priority reports.
- Automatic ticket ID generation using timestamp plus random suffix.
- Automatic local time and last-known GPS capture.
- Local SQLite storage for reports and ticket status lookup.
- Recent reports screen for reports saved on the phone.

## APK

Debug APK after build:

`app/build/outputs/apk/debug/app-debug.apk`

Install on a connected Android phone:

```powershell
adb install -r app/build/outputs/apk/debug/app-debug.apk
```

## Build

Open this folder in Android Studio and run the `app` configuration, or build from the command line:

```powershell
gradle assembleDebug
```

The app is written in Kotlin and targets Android SDK 35.
