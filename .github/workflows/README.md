# MusicU

A native Android music-player starter with a Material You-inspired interface.

## Build the APK using GitHub Actions (phone-friendly route)

1. Create a new, empty GitHub repository.
2. Extract this ZIP on your phone.
3. Upload the **contents of the `MusicU` folder**, keeping the folders and paths exactly as they are. Do not upload all files into the repository root flat. The `.github` folder contains the build workflow; make sure it is included (show hidden files in your file manager if necessary).
4. Open the repository's **Actions** tab. Select **Build MusicU APK**, then choose **Run workflow** if it has not started automatically.
5. When the run finishes successfully, open it and download the `MusicU-debug-apk` artifact.

## Project layout

```text
MusicU/
├── .github/workflows/build.yml
├── app/
│   ├── build.gradle.kts
│   └── src/main/
│       ├── AndroidManifest.xml
│       └── java/com/musicu/player/MainActivity.kt
├── build.gradle.kts
├── gradle.properties
└── settings.gradle.kts
```

## App scope

- Minimum Android version: Android 8.0 (API 26).
- Requests permission to read local audio files.
- Lists and plays local audio while the app is open.
- This starter does not yet include background playback, media notifications, playlists, album-art extraction, or persistent favourites.
