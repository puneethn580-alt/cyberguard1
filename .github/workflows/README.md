# CyberGuard (Android)
Background cyberbullying detection for all apps, with a floating ON/OFF button.

## Get the APK (pick one)
**A. No install - GitHub builds it for you**
1. Create a free GitHub repo, upload this whole folder (keep `.github/workflows`).
2. Open the repo -> Actions -> "Build APK" -> Run workflow (it also runs on every push).
3. When it finishes, download the `CyberGuard-apk` artifact -> unzip -> `app-debug.apk`.
**B. Android Studio:** File > Open this folder > Build > Build APK(s) > `app/build/outputs/apk/debug/app-debug.apk`.

## Install & use
Copy the APK to the phone, open it (allow "install unknown apps"). Open CyberGuard:
1. "Turn on detection service" -> Installed apps -> CyberGuard -> On. (reads text in other apps)
2. "Allow screen scanning" -> Start now. (checks text inside images and video)
Then use any app. HIGH-risk text is covered with a warning box; MEDIUM/ image-or-video text gets a coloured outline.
The round "Guard ON/OFF" button floats over every app: tap to switch protection on/off.

## Notes
* Everything runs on the phone. No text, image or video leaves the device.
* Android asks you to re-approve screen scanning after a reboot or when you stop it (Android security rule).
* Debug APK is fine for personal use; Google Play needs a signed release build and an accessibility-service declaration.
