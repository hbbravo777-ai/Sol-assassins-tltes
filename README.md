# SOUL ASSASSINS — Android Field Test 0.1

This repository contains the first mobile beta prototype and an Android WebView wrapper.

## What is included
- Browser-playable top-down field-test mission
- Android fullscreen landscape wrapper that auto-launches the mission
- Touch joystick and fire button
- WASD / arrow-key, mouse and Space controls on desktop
- Basic hostile AI, shooting, health, ammo, 3 intel pickups and extraction
- GitHub Actions workflow to compile a debug APK in the cloud

## Build APK from a phone
1. Open the **Actions** tab in this repository.
2. Select **Build Android Beta APK**.
3. Tap **Run workflow** on the main branch.
4. When the run completes, open it and download the `soul-assassins-beta-apk` artifact.
5. Extract the downloaded artifact ZIP and install `app-debug.apk` on Android. If prompted, allow installs from the browser/files app you used.

The APK is a debug build for testing, not a Play Store release. Android may show a warning because it is not Play Store distributed.

## Local browser test
Open `app/src/main/assets/index.html` in a modern browser, or use GitHub Pages after enabling it.

## Honest scope
This is an early 2D prototype, not the finished Unreal Engine 5 3D game. It does not include online/offline multiplayer, the 30 planned 3D maps, user accounts, voice chat, Solana wallet or purchases, production backend, anti-cheat, or an audited release. The APK build must complete successfully in Actions and then be installed and tested on a physical device before it can be called device-verified.

## Tech
Native Android shell: Java + Android WebView. Build: Gradle + Android Gradle Plugin. CI: GitHub Actions.
