# BrandMaster Sim Connect — Releases

Binary-only distribution repo for the BrandMaster Sim Connect Android app. No source code lives
here — just compiled, signed release APKs (under [Releases](../../releases)) and a small version
manifest (`latest.json`) that the app itself polls to check for updates.

## latest.json

```json
{"versionCode": 3, "versionName": "1.1.1", "apkUrl": "https://github.com/.../app-release.apk", "notes": "..."}
```

The app compares `versionCode` against its own `BuildConfig.VERSION_CODE` and offers a tap-to-install
update when this manifest describes a newer build.
