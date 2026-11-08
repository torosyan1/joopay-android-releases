# JooPay USSD Agent: releases

Built, signed APKs of the JooPay USSD Agent, published here by CI so phones can update
themselves from the app's **Update to latest version** button. No source code lives here.

- `latest.json` describes the newest release: `versionName`, `versionCode`, `apk` (path in
  this repo), `sha256`, `notes`, `publishedAt`.
- `apks/` holds the APK files.

The app downloads `latest.json`, installs the APK only when its versionCode is newer, its
sha256 matches, and it is signed with the same key as the installed app.
