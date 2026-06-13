# Civil Tools Releases

Official release repository for [Civil Tools](https://civil-tools.com) — an offline-first Android toolkit for civil engineers, architects, surveyors, contractors, and construction professionals.

## Releases

| Version | Date       | Status          | Download |
| ------- | ---------- | --------------- | -------- |
| v1.0    | 2025-06-13 | Initial Release | [Civil-Tools-v1.0.apk](./releases/v1.0/Civil-Tools-v1.0.apk) |

> **Note:** Each release folder under `releases/` contains the APK, a checksum file, and changelog.

## How to Publish a New Release

1. Build the signed APK from the main app repo.
2. Copy the APK into `releases/v<version>/`.
3. Generate the SHA-256 checksum:
   ```powershell
   Get-FileHash -Algorithm SHA256 releases/v<version>/Civil-Tools-v<version>.apk
   ```
4. Update the `CHANGELOG.md` with the new version details.
5. Update `RELEASE.env` with the latest version number.
6. Commit and push — the GitHub Release will be created automatically (if CI is set up).

## Repository Structure

```
civil-tools-releases/
├── releases/          # APK files organized by version
│   └── v1.0/
│       ├── Civil-Tools-v1.0.apk
│       └── Civil-Tools-v1.0.apk.sha256
├── screenshots/       # App screenshots for the website
├── assets/            # Branding files (logo, icons)
├── RELEASE.env        # Current release version variable
├── CHANGELOG.md       # Full version history
└── README.md
```

## Version History

See [CHANGELOG.md](./CHANGELOG.md) for the full release history.

## License

Copyright © Civil Tools. All Rights Reserved.
