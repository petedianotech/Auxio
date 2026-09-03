<p align="center"><img src="fastlane/metadata/android/en-US/images/icon.png" width="150"></p>
<h1 align="center"><b>Paimusic</b></h1>
<h4 align="center">Your local music player for Android</h4>

<p align="center">
    <img alt="Latest Version" src="https://img.shields.io/static/v1?label=tag&message=v1.1.0&color=64B5F6&style=flat">
    <img alt="License" src="https://img.shields.io/badge/license-GPL%20v3-2B6DBE.svg?style=flat">
    <img alt="Minimum SDK Version" src="https://img.shields.io/badge/API-24%2B-1450A8?style=flat">
</p>

## Paimusic

**Paimusic** is a fast, private, offline-first music player. It is based on the excellent Auxio codebase and is being developed further as a full-featured player with a cleaner identity.

- No "About" screen clutter — the app is focused on music
- Always displays as **Paimusic** (no Debug branding)
- Application ID: `org.paimusic.app`

### Current strengths
- Media3 / ExoPlayer engine
- Material 3 UI, edge-to-edge
- Gapless playback + full ReplayGain
- External equalizer support
- Folders, playlists, search, widgets, Android Auto
- Completely offline & private

### Roadmap (Poweramp-inspired)
Planned enhancements to bring more of the power users expect from high-end players like Poweramp:
- Stronger built-in EQ / tone controls and presets
- Crossfade & advanced gapless options
- Lyrics support
- More playback / library customization
- Improved visualizations and player UI polish

## Building

GitHub Actions builds a debug APK on every push to `dev` and uploads the artifact **Paimusic-debug**.

Local requirements: `cmake`, `ninja-build`, JDK 21, submodules.

```bash
git clone --recurse-submodules https://github.com/petedianotech/Auxio.git
cd Auxio
./gradlew app:assembleDebug
```

## License

GNU GPLv3 (same as the original Auxio project).

---

Maintained by [petedianotech](https://github.com/petedianotech). Original Auxio by Alexander Capehart / OxygenCobalt.
