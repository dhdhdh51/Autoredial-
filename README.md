# Safe Call Reminder

A safe Android assignment project that helps you call a number and manually retry if the call was busy, cut, or not answered.

## Safety note
This app intentionally does **not** do continuous hidden auto-calling or auto-redial loops. It opens the Android dialer with the number, then the user manually presses call. After the call, return to the app and choose:

- **Answered → Finish**
- **Busy / Cut / No Answer → Retry**
- **Stop Task**

## Features

- Phone number input
- Retry delay input
- Maximum retry limit
- Beautiful simple UI
- No dangerous call permission required
- GitHub Actions workflow to build debug APK

## Build on GitHub

1. Upload all files to a GitHub repository.
2. Go to **Actions** tab.
3. Open **Android Debug APK Build** workflow.
4. Click **Run workflow** or push code to `main`.
5. Download APK from workflow **Artifacts**.

## Local build

```bash
gradle :app:assembleDebug
```

Output:

```text
app/build/outputs/apk/debug/app-debug.apk
```
