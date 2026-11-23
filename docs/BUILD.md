# Build from source

## Requirements

- JDK 21
- Android SDK and NDK versions required by the Gradle project, plus CMake
- Git with recursive submodule support
- Network access to download Gradle dependencies and the upstream Java 8 runtime package

## Windows

1. Clone this repository with submodules: `git clone --recursive https://github.com/cop3465cy-dotcom/blockside-android.git`
2. Download the public `jre8-pojav` artifact from the upstream OpenJDK build workflow and extract it into `app_pojavlauncher/src/main/assets/components/jre/`. See [Amethyst's build notes](https://github.com/AngelAuraMC/Amethyst-Android/blob/v3_openjdk/README.md#building).
3. Run `scripts\languagelist_updater.bat`.
4. Run `gradlew.bat :app_pojavlauncher:assembleDebug`.
5. Find the APK at `app_pojavlauncher\build\outputs\apk\debug\app_pojavlauncher-debug.apk`.

Do not put the checkout in a path containing spaces; the upstream native build notes warn that ndk-build can fail on such paths. Do not add signing keys, API tokens, or downloaded runtime bundles to commits.

GitHub Actions uses Ubuntu, JDK 21, Gradle 9.6.1, recursive submodules, and the public upstream `jre8-pojav` CI artifact. It builds a debug APK and publishes it as a short-lived Actions artifact; it does not create a Play Store signed build.
