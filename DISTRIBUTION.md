# StreamFlow TV updates

This repository distributes StreamFlow TV beta APKs and update metadata. Source code and signing keys are not stored here.

## First release
Create a Release tagged `v0.2.0`, titled `StreamFlow TV 0.2.0`. Attach both `StreamFlow-TV-0.2.0.apk` and `update.json` from the prepared release folder. Publish as Latest, not pre-release.

The app reads `https://github.com/svenna123456/streamflow-tv-updates/releases/latest/download/update.json`. That file must point to the matching versioned APK release asset and include its exact byte size and SHA-256. Keep both assets available and do not replace existing version bytes. Later releases require increasing versionCode and the same signing certificate.

Version 0.2.0 is the initial OTA-capable beta. Older installations need this APK once; later updates can be downloaded in the app. Android asks the user to approve installation. Source permission may need enabling for StreamFlow on the device.

The first assets are prepared locally but have not yet been uploaded or published. The presence of this document alone does not activate the feed.
