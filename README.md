# The Pastor's Kid - Native Android Application

A native Android story reader and audiobook application for **"The Pastor's Kid"** by Frent Mwendwa, built with **Kotlin** and **Jetpack Compose** (Material 3).

## Key Features
- **100% Offline Story**: Complete unabridged 11 chapters bundled locally into native Kotlin models.
- **Offline Audio Narration**: Powered by Android's native `android.speech.tts.TextToSpeech` engine. Operates completely without internet.
- **Synchronized Text Highlighting**: Real-time paragraph highlighting matching the audio narration.
- **Table of Contents & Navigation**: Quick-drawer navigation across all 11 chapters with completion badges.
- **Customization**: Three reading themes (Sepia, Dark, Light), adjustable font size (14sp to 26sp), and variable speech rate (0.75x to 2.0x).
- **Persistent Bookmarks**: Remembers your exact reading spot and settings across app restarts using SharedPreferences.

---

## How to Build the Real Android APK (.apk)

### Option 1: Using Android Studio (Recommended)
1. Open **Android Studio** (Koala, Ladybug, or newer).
2. Select **Open** and choose this `android/` folder.
3. Wait for Gradle sync to complete.
4. In the top menu, go to **Build** &rarr; **Build Bundle(s) / APK(s)** &rarr; **Build APK(s)**.
5. Once built, click **"locate"** in the popup to get your installable:
   `app/build/outputs/apk/debug/app-debug.apk`
6. Transfer this `.apk` to any Android phone and install it directly!

### Option 2: Using Command Line (Terminal)
Ensure you have JDK 17 or 21 and the Android SDK installed:
```bash
./gradlew assembleDebug
```
The output APK will be generated at:
```bash
app/build/outputs/apk/debug/app-debug.apk
```

---

## Technical Specifications
- **Language**: Kotlin 2.0.21
- **UI Framework**: Jetpack Compose (BOM 2024.11.00) with Material 3
- **Android Gradle Plugin**: 8.7.3
- **Minimum SDK**: Android 8.0 (API 26)
- **Target SDK**: Android 15 (API 35)
- **Speech Engine**: `android.speech.tts.TextToSpeech`
