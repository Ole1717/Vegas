# Vegas - AI Agent for Android

**Vegas** is an AI-powered file management and coding agent for Android. It understands natural language commands and performs file operations, project creation, and coding tasks on your device.

## Project Structure

```
vegas-android/
├── app/                          # Main app module
│   ├── src/main/
│   │   ├── java/com/vegas/agent/ # Kotlin source code
│   │   ├── res/                  # Resources (layouts, strings, colors)
│   │   └── AndroidManifest.xml
│   └── build.gradle.kts
├── gradle/wrapper/               # Gradle Wrapper
├── .github/workflows/            # GitHub Actions CI/CD
├── build.gradle.kts              # Root build config
├── settings.gradle.kts           # Project settings
└── gradle.properties             # Gradle properties
```

## Build Configuration

- **Android Gradle Plugin**: 8.3.0
- **Gradle**: 8.6
- **Kotlin**: 1.9.23
- **Compile SDK**: 35 (Android 15)
- **Min SDK**: 26 (Android 8)
- **Target SDK**: 35
- **JDK**: Java 11

## Building APK

### Using GitHub Actions (Recommended)

Push to `main` branch or manually trigger workflow:

1. Go to Actions tab
2. Select "Build Vegas APK"
3. Click "Run workflow"
4. Download artifact from completed workflow

APK will be available as `Vegas-debug.apk`

### Local Build (Termux)

```bash
cd ~/vegas-android
./gradlew assembleDebug
```

APK will be at: `app/build/outputs/apk/debug/app-debug.apk`

## Development

### Prerequisites

- Android SDK (API 35)
- JDK 11
- Git

### First Time Setup

```bash
git clone https://github.com/YOUR_USERNAME/vegas-android.git
cd vegas-android
./gradlew build
```

## Contributing

All changes should trigger GitHub Actions build automatically.

Check Actions tab to ensure BUILD SUCCESSFUL ✓

## License

MIT
