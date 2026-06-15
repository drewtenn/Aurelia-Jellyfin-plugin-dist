# Media Stream Filters — Jellyfin plugin repository

Public **plugin repository** (manifest + release artifacts) for the
**Media Stream Filters** Jellyfin server plugin. The plugin source lives in a
private repository; this repo hosts only the published `manifest.json` and the
compiled plugin zips so Jellyfin can install and update them.

## Install in Jellyfin

**Dashboard → Plugins → Repositories → Add**, then add this repository URL:

```
https://raw.githubusercontent.com/drewtenn/Aurelia-Jellyfin-plugin-dist/main/manifest.json
```

Then open **Catalog**, install **Media Stream Filters**, and restart Jellyfin.

## What the plugin does

Server-side library filtering by media-stream characteristics Jellyfin's core
API can't express — video dynamic range (SDR/HDR10/HDR10+/Dolby Vision/HLG),
video codec, audio codec, audio channel count, and spatial audio (Dolby Atmos /
DTS:X) — via a paginated `BaseItemDto`-compatible endpoint plus a capability
endpoint for client feature-detection.
