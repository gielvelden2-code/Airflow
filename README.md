# AirFlow Android MVP

This is a **functional prototype**, not a complete AirDrop replacement.

## What works
- Android share sheet: Gallery -> Share -> AirFlow
- Share one or multiple files via a local Wi-Fi HTTP web page
- Other devices (iPad, iPhone, Mac, Windows) can use Safari/Chrome to download shared files or upload files to Android
- No cloud file storage

## Build APK using only an Android phone
1. Upload the **contents** of this ZIP to the root of a GitHub repository (not inside an extra folder).
2. Open GitHub Actions -> Build AirFlow APK -> Run workflow.
3. Download the artifact `AirFlow-debug-APK`, unzip, install `app-debug.apk` on Android.
4. Android and receiving device must be on the same Wi-Fi. Open AirFlow and share a file. The displayed URL is accessible from the other device's browser.

## Limitations
- Android must keep the app open while sharing.
- No native iPad/Windows/Mac app, automatic nearby discovery, or background reception.
- Uses unencrypted local HTTP. Use only on a trusted Wi-Fi network; anyone on the LAN with the URL can access files.
- Debug build only; not production-ready. The APK has not been device-tested here.
