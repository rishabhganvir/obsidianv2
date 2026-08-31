# OBSIDIAN

Premium mobile workout tracker built with Expo SDK 57, React Native 0.86, TypeScript, and the New Architecture.

## Run locally

```bash
npx expo install
npx expo start
```

## Build an Android APK from GitHub

Push this folder to a GitHub repository. The included GitHub Action makes the installable APK automatically on every push to `main`.

1. Open the repository's **Actions** tab.
2. Select **Build Android APK** and open the newest run.
3. Download `obsidian-debug-apk` from **Artifacts**.

For a signed Play Store bundle, use Expo's managed cloud builder:

```bash
npm install --global eas-cli
eas login
eas init
eas build --platform android --profile production
```

`eas init` replaces `REPLACE_AFTER_EAS_INIT` in `app.json` with your EAS project ID.

## Calories

Food search uses the public Open Food Facts search endpoint. Food records are stored locally on the device, with manual calorie entry always available.
