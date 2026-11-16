# Quran for Windows and Android

A Quran reader and recitation player: the mushaf page as printed, recitations by well-known reciters that follow along word by word, tafsir and translations, bookmarks, and memorisation practice. Everything you download stays on your device and works offline.

- **Text:** the King Fahd Complex (KFGQPC) Hafs edition, shown in its own font. The apps check the text files when they start and refuse to run if they have been changed.
- **Riwayah:** Hafs from Asim.
- **Help:** each app has a guided tour and a Help page (English and Bangla).

## Download

Open **[Releases](../../releases)** and pick the newest release for your device. The files are under **Assets**.

| Device | File | Notes |
|---|---|---|
| Windows 10 / 11 (64-bit) | `Quran_<version>_x64-setup.exe` | Recommended. Installs for you only; no administrator rights needed. |
| Windows, all users | `Quran_<version>_x64_en-US.msi` | Installs in Program Files for everyone on the PC; needs administrator rights. |
| Android 8.0 or newer | `Quran-<version>.apk` | Install directly on the phone (see below). |

Windows releases are tagged `windows-v…` and Android releases `android-v…`.

## Installing on Windows

1. Download the `setup.exe` and open it.
2. The installer is not code-signed yet, so Windows SmartScreen may say **"Windows protected your PC"**. Choose **More info**, then **Run anyway**.
3. WebView2 is downloaded during setup if it is missing (Windows 11 already has it).

To update, install the newer version over the old one; your bookmarks and settings are kept.

## Installing on Android

1. Open the release on your phone and tap the `.apk` file to download it.
2. Open the file. Android asks you to allow your browser (or file manager) to **install unknown apps**: allow it for this install.
3. If Google Play Protect warns that the app is unknown, choose **Install anyway**. The app is not on Google Play yet.

Later versions install over the earlier one and keep your bookmarks, progress and downloads.

## Checking a download

Each release has a `SHA256SUMS.txt`. To check a file:

- Windows: `certutil -hashfile Quran_<version>_x64-setup.exe SHA256`
- Linux / macOS: `sha256sum -c SHA256SUMS.txt`

## Reporting a problem

Open an [issue](../../issues) with your device, the app version and what happened.
