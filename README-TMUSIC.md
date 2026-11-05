# Tmusic

Custom build of [Myspoti](https://github.com/kota-zo/myspoti) (GPL-3.0) with:

- **App name:** Tmusic (`app.tmusic` / `app.tmusic.stable`)
- **Default UI:** Immersive look (large art, glass chrome, iOS-style settings)
- **Icon:** Red “T” launcher mark
- **Downloads:** Use **Settings → Extensions** to install a **download-source** extension, then **Download** on any song (⋮ menu) or from album/playlist actions

## Build (debug APK)

Requirements: JDK 17+, Android SDK.

```bash
cd base
./gradlew assembleDebug
```

APK: `base/app/build/outputs/apk/debug/app-debug.apk`

On Windows:

```powershell
cd base
.\gradlew.bat assembleDebug
```

Install on a device with USB debugging, or copy the APK to the phone.

## Notes

- You still **log in with Spotify**; playback uses the official Web Player bridge.
- **GPL-3.0:** If you distribute this APK, you must provide corresponding source (this repo).
- Upstream update checks are disabled for local builds unless you set `-PupdateRepo=...` in CI.
- For a sharper custom logo, replace `base/app/src/main/res/drawable/ic_launcher_foreground.xml` or use Android Studio **Image Asset**.

## What we changed vs upstream

See git history on this fork. Main touchpoints:

- `base/app/build.gradle.kts` — application id and label
- `base/app/src/main/java/.../LookPref.kt` — default Immersive
- `base/app/src/main/res/values/myspoti_strings.xml` — Tmusic branding strings
- `base/app/src/main/res/drawable/ic_launcher_*.xml` — icon
