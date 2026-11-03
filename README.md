TV App Hub — KitKat Edition

A remote-first Android app catalogue designed for Android 4.4.4 (API 19) TVs.

## Controls

- D-pad arrows: move between the menu, cards, and actions.
- OK / Select / Enter: open the selected card or action.
- Back: return from an app download page to the hub.
- No mouse or touchscreen is required for the hub interface.

## What is included

- Crosswalk Project Runtime is included as a dedicated catalogue entry.
- VLC media player catalogue page with Android 4.2+ builds; select the TV’s matching CPU variant.
- TV Bro is shown as incompatible rather than offering a misleading KitKat download: current listed releases require Android 7.0+ .
- Uptodown and F-Droid web catalogues for finding additional apps.
- Add App form: save any HTTPS app download page to the local catalogue. An optional direct APK URL can be sent to Android Download Manager.
- APK downloads opened from supported web pages are handed to Android Download Manager and shown in the system Downloads screen.

## Important notes

1. Crosswalk is a legacy runtime component, not a normal app. It has no launcher icon and normally only needs to be installed when another app specifically asks for it. Its archive offers multiple old builds/architectures; select a build that matches the TV.
2. APKs must match both the TV's Android version and CPU architecture (for example, ARMv7, ARM64, or x86). An APK can still fail even when the Android version looks compatible.
3. Installing an APK is always confirmed by Android's package installer. The hub does not silently install apps or bypass Android security settings.
4. On Android 4.4, the system may require the user to enable installation from unknown sources in Settings before manually installing a downloaded APK. Only install files from a source you trust.
5. App pages are live web pages and can change. The built-in catalogue is intentionally small; use Add App to save other HTTPS download pages.

## Build the Android APK

This folder is an Android Studio project, not a prebuilt APK. To build it:

1. Open this folder in Android Studio on a computer.
2. Install Android SDK Platform 33 and a JDK 11-compatible Android Gradle Plugin environment.
3. Let Android Studio sync Gradle, then choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. Copy the generated APK to the TV and open it with the TV's file manager or Downloads app.

The app's minimum Android version is API 19 (Android 4.4 / KitKat). It is not possible to install this app on Android versions older than 4.4.
