# LinDirStat releases

Downloads of [LinDirStat](https://github.com/danjboyd/LinDirStat), a disk
usage viewer for Linux and macOS modelled on WinDirStat. The source code,
screenshots and documentation are in
[danjboyd/LinDirStat](https://github.com/danjboyd/LinDirStat).

Each [release](https://github.com/danjboyd/LinDirStat-releases/releases/latest)
has a Linux AppImage and a macOS disk image.

## Linux

Download `LinDirStat-<version>-x86_64.AppImage`, make it executable, and run
it:

```sh
chmod +x LinDirStat-*-x86_64.AppImage
./LinDirStat-*-x86_64.AppImage
```

The AppImage needs 64-bit Linux with glibc 2.38 or newer and GTK 4, for
example Debian 13, Ubuntu 24.04 or newer, or Fedora 39 or newer. It has been
tested on Debian 13. It does not need FUSE 2; without FUSE, run it with
`--appimage-extract-and-run`.

### Updates

LinDirStat checks this repository for new releases and offers to install them
(**Help › Check for Updates…**). Updates are signed, and an AppImage whose
signature doesn't match is refused. The update feed is published here on
GitHub Pages (`updates/linux/stable.json`). AppImageUpdate and AppImageLauncher
can also update the AppImage.

## macOS

Download `LinDirStat-<version>-macos-universal.dmg` (macOS 13 or newer, Apple
Silicon and Intel), open it, and drag LinDirStat to Applications.

The app is not notarized by Apple yet, so the first launch is blocked. Open it
once, then click **Open Anyway** in **System Settings › Privacy & Security**,
or run:

```sh
xattr -dr com.apple.quarantine /Applications/LinDirStat.app
```

The macOS app does not update itself yet; new versions appear here.

## License

LinDirStat is GPL-2.0-or-later. Each package carries its license and the
notices of the components it bundles.
