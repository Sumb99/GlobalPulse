# GlobalPulse Android MVP

This is the first offline Android MVP. It is intentionally dependency-light so it can be built reliably.

## Current app
- GlobalPulse branding
- Home / Trending / category tabs (UI)
- News cards
- Refresh action
- Offline demo stories
- Android INTERNET permission already prepared for the next live-data phase

## Planned live pipeline
GDELT/RSS -> Supabase Edge Function -> Supabase Database -> duplicate detection -> story clustering -> trend score -> Android app -> notifications -> AdMob.

## Build the APK
The included GitHub Actions workflow builds `app-debug.apk` automatically using Android SDK 35 and Gradle 8.9. No Android Studio is required for the cloud build.

### Easiest environment
1. Create a GitHub repository.
2. Upload this entire project.
3. Open **Actions** and run **Build GlobalPulse APK**.
4. Open the completed workflow run.
5. Download the artifact **GlobalPulse-v1.0-debug**.
6. Extract it and install `app-debug.apk` on the Samsung phone.

For local building, use Android Studio with JDK 17, Android SDK Platform 35 and Build Tools 35.0.0.
