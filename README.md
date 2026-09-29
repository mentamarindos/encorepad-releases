# EncorePad downloads

This repository is a **download mirror**. It holds the built EncorePad installers
and nothing else. No source code lives here.

The source is private. Every release here is built and published by the release
workflow in the source repository.

## What you can download

Each GitHub Release in this repository holds the Windows build for one version:

- `encorepad_<version>_x64-setup.exe` — the installer. **This is the recommended
  download.** It installs EncorePad properly and keeps itself up to date.
- `encorepad_<version>_x64-portable.zip` — a single executable that runs without
  installing. Use it when you cannot install software. Replace the file by hand
  when a new version arrives.
- `SHA256SUMS.txt` — checksums for every file in the release.

## Verifying a download

```powershell
Get-FileHash .\encorepad_0.22.0_x64-setup.exe -Algorithm SHA256
```

Compare the result against the matching line in `SHA256SUMS.txt`.

## Other mirrors

The installer is also published to Cloudflare R2 and to the project's download
page. If a download fails here, try the download page linked from
[encorepad.plyntar.com](https://encorepad.plyntar.com).
