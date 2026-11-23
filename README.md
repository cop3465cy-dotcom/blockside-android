# Blockside for Android

Blockside is an Android launcher interface built on the maintained Amethyst Android Java Edition launcher engine. It is a real launcher project, not a Minecraft game binary or a mockup. It includes the launcher and runtime integration; it does not include Minecraft game files.

> **Compatibility:** Android 5.0 (API 21) or newer. Minecraft version and device compatibility depend on the selected Java runtime, graphics driver, available memory, and the upstream engine.

## What this project provides

- A custom Blockside home screen, profile surface, recent-world list, quick actions, and launcher icon.
- The Amethyst/Pojav-based Java Edition launcher engine, including its account, version, mod-loader, runtime, rendering, and input integrations.
- Local offline username profiles for single-player with game versions already installed on the device.
- Android builds under application ID `com.cop3465cy.blockside`.

The interface, launcher engine, installed game, and game engine are distinct pieces. This app supplies the launcher and integrates a compatible Java runtime. Minecraft itself is downloaded through the launcher after Microsoft sign-in; the game is proprietary software and is not bundled here. Offline profiles do not sign in, grant ownership, unlock downloads, or authenticate multiplayer servers. Java Edition is executed through Android-compatible runtime and graphics layers. This is not Mojang/Microsoft software and is not affiliated with them.

## Install

See [Android installation guide](docs/INSTALL.md). Debug APKs use Gradle's debug signing key for installable previews. GitHub Actions generates its own key; each run can have a different signature, so a new preview may require uninstalling the previous build first. Do not use preview builds as production releases.

## Build

See [build guide](docs/BUILD.md). Builds need JDK 21, Android SDK/NDK and CMake, the checked-in Gradle wrapper, recursive Git submodules, and the upstream JRE asset package. GitHub Actions produces a preview APK artifact.

## Project docs

- [Installation](docs/INSTALL.md)
- [Build from source](docs/BUILD.md)
- [Compatibility and limitations](docs/COMPATIBILITY.md)
- [Upstream notices and licensing](UPSTREAM-NOTICES.md)
- [Privacy policy](GPLAY_PRIVACY_POLICY)

## License

This fork is distributed under the GNU Lesser General Public License v3.0, as required by the upstream project. See [LICENSE](LICENSE) and [UPSTREAM-NOTICES.md](UPSTREAM-NOTICES.md). Minecraft and related marks belong to their respective owners.
