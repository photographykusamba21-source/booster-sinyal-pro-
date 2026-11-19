# BOOSTER SINYAL PRO — STANDARD v4.0

Android app for practical, non-root cellular connection optimization. Target use: Vivo Y75 5G / Android 14 / Smartfren 4G and 5G, mobile data only.

## What the app does
1. Reads Android-exposed LTE/NR cell signal metrics where available (dBm, RSRP, RSRQ, SINR).
2. Diagnoses likely weak radio reception versus possible network congestion/latency problems.
3. Runs latency, download and upload tests using the currently active cellular `Network`, not Wi-Fi. It refuses to start if Android reports Wi-Fi as the active connection.
4. Gives practical actions: move to a better reception position, manually refresh mobile radio through Airplane Mode settings, and compare before/after results.
5. Opens Android network settings for actions that require system privileges.

## What it cannot do
A normal Android app cannot increase antenna gain, modem transmit power, receiver sensitivity, force LTE/5G bands, force a 5G attach, or toggle Airplane Mode/mobile data silently on modern Android. Those require hardware, OEM/carrier privileges, or user action. This app does not fake a BOOST effect.

## Data usage
A test targets approximately 3 MB download + 1 MB upload plus small latency requests. Actual transfer may vary. Tests consume mobile data. Cloudflare public speed-test endpoints are used; server/routing availability affects results.

## Build from an Android phone using GitHub
1. Extract this ZIP on the phone.
2. In your GitHub repository, upload the **contents** of the extracted folder to the repository root. Preserve the `.github/workflows` directory.
3. Commit to your main branch.
4. Open Actions → `Build BOOSTER SINYAL PRO Standard APK`.
5. Open the successful run and download artifact `BOOSTER-SINYAL-PRO-standard-debug-apk`.
6. Extract the artifact ZIP and install `app-debug.apk`.

No Wi-Fi is needed to run the app. GitHub build and download need internet; mobile data is enough.
