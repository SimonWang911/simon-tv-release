# Simon TV Release

This repository hosts public update manifests and GitHub Release assets for Simon TV.

## Update Manifests

- `apk/mobile.json`
- `apk/leanback.json`

The app reads the manifest for its current mode, compares `code` with the installed `versionCode`, and downloads the matching ABI APK from the release asset URLs.

## Release Asset Names

- `Simon-mobile-arm64_v8a.apk`
- `Simon-mobile-armeabi_v7a.apk`
- `Simon-leanback-arm64_v8a.apk`
- `Simon-leanback-armeabi_v7a.apk`

## Proxy Prefix Order

The app tries the original GitHub Release asset URL first, then proxy-prefixed URLs in manifest order:

1. `https://gh-proxy.com/`
2. `https://wget.la/`
3. `https://ghfast.top/`
