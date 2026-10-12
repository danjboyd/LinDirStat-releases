# LinDirStat releases

Linux builds of LinDirStat, a GNUstep disk usage viewer modelled on
WinDirStat. Each release has an x86_64 AppImage.

## Install

Download `LinDirStat-<version>-x86_64.AppImage` from the latest release, make
it executable, and run it:

```sh
chmod +x LinDirStat-*-x86_64.AppImage
./LinDirStat-*-x86_64.AppImage
```

The AppImage needs a desktop with GTK 4 and glibc 2.41 or newer (Debian 13 or
later). LinDirStat is GPL-2.0-or-later; each AppImage carries its licence and
the notices of the components it bundles.

## Updates

LinDirStat checks this repository for new releases and offers to install them
(**Help › Check for Updates…**). Updates are signed, and an AppImage whose
signature doesn't match is refused. The update feed is published here on
GitHub Pages (`updates/linux/stable.json`). AppImageUpdate and AppImageLauncher
can also update the AppImage.
