# SuperFly releases

Downloads for SuperFly software.

## SuperFly Manager

SuperFly Manager (`sfm`) deploys and manages SuperFly HTML Engine containers on your hosts.

[Documentation](https://docs.superfly.tv/html-engine) · [Host setup](https://docs.superfly.tv/html-engine/host-setup/host-setup) · [All releases](https://github.com/SuperFlyTV/SuperFly-releases/releases)

### Install

macOS (Apple Silicon) and Linux, with [Homebrew](https://brew.sh):

```sh
brew install superflytv/tap/sfm
```

Windows:

```powershell
winget install SuperFlyTV.SuperFlyManager
```

Update later with `brew upgrade sfm` or `winget upgrade SuperFlyTV.SuperFlyManager`.

### Start

In an empty directory for your configuration, run:

```sh
sfm ui
```

Open the URL it prints and follow **Getting started** to add hosts and configure your engines.

Requires Git and SSH locally, and Docker on the managed hosts. Running the HTML Engine requires an engine license.

### Without a package manager

Download `sfm` for your OS from the [latest release](https://github.com/SuperFlyTV/SuperFly-releases/releases/latest), check it against `SHA256SUMS`, rename it to `sfm` (`sfm.exe` on Windows) and put it on your `PATH`. On Linux, make it executable with `chmod +x sfm`.
