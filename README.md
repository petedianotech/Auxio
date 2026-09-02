<p align="center"><img src="fastlane/metadata/android/en-US/images/icon.png" width="150"></p>
<h1 align="center"><b>Paimusic</b></h1>
<h4 align="center">A simple, rational music player for Android (based on Auxio).</h4>

<p align="center">
    <img alt="Latest Version" src="https://img.shields.io/static/v1?label=tag&message=v1.0.0&color=64B5F6&style=flat">
    <img alt="License" src="https://img.shields.io/badge/license-GPL%20v3-2B6DBE.svg?style=flat">
    <img alt="Minimum SDK Version" src="https://img.shields.io/badge/API-24%2B-1450A8?style=flat">
</p>

## About

**Paimusic** is a local music player forked and continued from [Auxio](https://github.com/OxygenCobalt/Auxio). It keeps the same clean, rational design and modern Media3-based playback while being rebranded and prepared for further improvements.

It plays music. Fast UI, excellent library support, gapless playback, ReplayGain, Android Auto, widgets, and complete offline privacy.

**Original project:** [OxygenCobalt/Auxio](https://github.com/OxygenCobalt/Auxio) by Alexander Capehart.

## Features

- Playback based on Media3 ExoPlayer
- Snappy Material Design 3 UI
- Opinionated UX focused on ease of use
- Customizable behavior
- Support for disc numbers, multiple artists, release types, precise dates, sort tags, and more
- Advanced artist system
- SD Card-aware folder management
- Reliable playlists
- Playback state persistence
- Android Auto support
- Automatic gapless playback
- Full ReplayGain support
- External equalizer support
- Edge-to-edge, embedded covers, search, headset autoplay, adaptive widgets
- Completely private and offline

## Building / CI

A GitHub Actions workflow (`.github/workflows/android.yml`) automatically builds a **debug APK** on every push to `dev`/`main` and uploads it as an artifact named `Paimusic-debug`.

You can also trigger it manually via the Actions tab.

### Local build requirements

- `cmake` and `ninja-build`
- JDK 21
- Submodules: `git clone --recurse-submodules`

```bash
./gradlew app:assembleDebug
```

The debug APK will be at `app/build/outputs/apk/debug/`.

## License

Same as the original Auxio project: GNU GPLv3.

---

*Paimusic is a community continuation / rebrand of Auxio for further development under the Paimusic name.*
