# Nottify

An independent music player for Android, built with Kotlin, Jetpack Compose and Media3.

This repository is open source under the [MIT license](LICENSE).

## Building

1. Open the project in Android Studio (Hedgehog or newer), or build from the command line:
   ```bash
   ./gradlew :app:assembleProdRelease
   ```
2. The Android SDK path is read from `local.properties` (`sdk.dir=...`) or `ANDROID_HOME`.
3. Release signing is optional. Copy `keystore.properties.example` to `keystore.properties`, create your own keystore, and fill in the passwords. Without it, the build still produces an unsigned APK.

Signed APKs for each release are published on the [Releases](../../releases) page.

## Releases

Version names and codes are set in `app/build.gradle.kts`. The app package is
`com.horrockstom26.spotify` (kept stable so existing installs can update).

## Notes

- Some source files contain historical branding strings from earlier versions of the project.
- Third-party services (YouTube Music, Spotify, Last.fm, Discord, etc.) are accessed through their public endpoints; no credentials are bundled in this repository.
