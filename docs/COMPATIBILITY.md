# Compatibility and limitations

- Minimum Android version: 5.0 (API 21), as configured by the inherited launcher engine. Modern Android devices are recommended for memory and graphics compatibility.
- Java Edition versions require a compatible runtime; version availability and loader support depend on the upstream Amethyst engine and selected Java runtime.
- Performance varies with chipset, Android graphics drivers, memory, resolution, and renderer. A compatible device is not guaranteed to run every version or mod.
- Microsoft account authentication is handled by the inherited launcher flow and its browser/device integration. An offline/local profile is not an authenticated Microsoft account and does not grant access to licensed game downloads or online services.
- World discovery reads worlds accessible to the launcher's game directory. Back up worlds before moving data or uninstalling preview builds.
- No Minecraft game data, official account credentials, or official signing keys are stored in this repository.

This repository changes the launcher presentation and Android application ID while using the upstream Java launcher implementation. It does not reimplement Mojang's game engine.
