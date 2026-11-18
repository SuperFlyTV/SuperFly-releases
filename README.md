# SuperFly releases

Downloads for SuperFly software.

## SuperFly Manager

SuperFly Manager (`sfm`) deploys and manages SuperFly HTML Engine containers on your hosts.

[Documentation](https://docs.superfly.tv/html-engine) · [Host setup](https://docs.superfly.tv/html-engine/host-setup/host-setup) · [All releases](https://github.com/SuperFlyTV/SuperFly-releases/releases)

### Install

#### macOS (Apple Silicon) and Linux

With [Homebrew](https://brew.sh):

```sh
brew install superflytv/tap/sfm
```

Update later with `brew upgrade sfm`.

#### Windows

<!-- Not in winget yet: restore once SuperFlyTV.SuperFlyManager is merged into microsoft/winget-pkgs.
```powershell
winget install SuperFlyTV.SuperFlyManager
```

Update later with `winget upgrade SuperFlyTV.SuperFlyManager`.
-->

Download `sfm-windows-amd64-setup.exe` from the [latest release](https://github.com/SuperFlyTV/SuperFly-releases/releases/latest) and run it. It needs no admin, and puts `sfm` on your `PATH` for any terminal opened afterwards. Update later by running a newer installer. To uninstall, find SuperFly Manager in Settings > Apps > Installed apps.

### Start

In an empty directory for your configuration, run:

```sh
sfm ui
```

Open the URL it prints and follow **Getting started** to add hosts and configure your engines.

Requires Git and SSH locally, and Docker on the managed hosts. Running the HTML Engine requires an engine license.

### Without a package manager

Download the `sfm` binary for your OS from the [latest release](https://github.com/SuperFlyTV/SuperFly-releases/releases/latest), check it against `SHA256SUMS`, rename it to `sfm` (`sfm.exe` on Windows) and put it on your `PATH`. On Linux, make it executable with `chmod +x sfm`.
