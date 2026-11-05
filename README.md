# Tmusic

[![Release](https://img.shields.io/github/v/release/Anilkumar01739/Tmusic?label=download)](https://github.com/Anilkumar01739/Tmusic/releases/latest)
[![License: GPL-3.0](https://img.shields.io/github/license/Anilkumar01739/Tmusic)](LICENSE)

**Tmusic** is a Spotify client for Android with an **iPhone-style Immersive UI**, ad blocking on a free account, and **offline downloads** through installable extensions. Sign in with your normal Spotify account; Tmusic never sees your password.

| | |
|---|---|
| **App name** | Tmusic |
| **Package** | `app.tmusic` (debug builds) / `app.tmusic.stable` (release builds) |
| **Default look** | Immersive — large artwork, glass bars, animated lyrics |
| **Android** | 10+ (API 29+) |

<p align="center">
  <a href="https://github.com/Anilkumar01739/Tmusic/releases/latest"><b>⬇ Download the latest APK</b></a>
</p>

## Install

1. Open the [latest release](https://github.com/Anilkumar01739/Tmusic/releases/latest) and download **`app-debug.apk`** (or the attached release APK).
2. Allow installs from your browser or file manager when Android asks.
3. Open **Tmusic** → **Log in with Spotify**.
4. Complete setup (quality, permissions). The **Immersive** look is already the default.

## Download songs

Tmusic does not ship a built-in download server. To save tracks offline:

1. **Settings → Extensions** → install a **download-source** extension (community repos use the topic `myspoti-extension` on GitHub).
2. On any song, open the **⋮** menu → **Download** (albums and playlists support bulk download too).
3. Files stay **encrypted inside the app** on your phone.

## Features

- Spotify home, search, library, playlists, Connect, Android Auto
- No audio/video ads on a free account (via the official Web Player bridge)
- Word-by-word lyrics, music videos, Genius song meanings
- Reorder playback sources in **Settings → Playback**
- Classic look still available under **Settings → Display**

## Build from source

Requirements: **JDK 17+**, **Android SDK**.

```powershell
cd base
.\gradlew.bat assembleDebug -Pabis=arm64-v8a
```

Output: `base/app/build/outputs/apk/debug/app-debug.apk`

See [`README-TMUSIC.md`](README-TMUSIC.md) for fork-specific notes.

## Upstream & license

Tmusic is a **fork** of [Myspoti](https://github.com/kota-zo/myspoti) and remains under **GPL-3.0**. You must keep copyright and license notices, credit [Myspoti](https://github.com/kota-zo/myspoti) as the origin, and publish complete source for any APK you distribute.

## Credits

- Based on [Myspoti](https://github.com/kota-zo/myspoti) (GPL-3.0)
- UI lineage: [Spotui](https://github.com/Spotui/Spotui) / [Metrolist](https://github.com/MetrolistGroup/Metrolist); Immersive look from [BitChord](https://github.com/kushagrasinghx/BitChord)
- Full notices: [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md)

## License

GPL-3.0 — see [`LICENSE`](LICENSE) and [`AGENTS.md`](AGENTS.md).
