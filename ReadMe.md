
![image](https://user-images.githubusercontent.com/130898607/232394911-0cd23d72-350f-46ed-8976-185b0686f374.png)


# GuidedFlipper Filmware. 
### made with love from jake.


## I need help

The best place to search for answers is the flipper docs [User Documentation](https://docs.flipperzero.one). If you can't find the answer there, check the flipper [Discord Server](https://flipp.dev/discord) or the [Forum](https://forum.flipperzero.one/).



## Requirements

Supported development platforms:

- Windows 10+ with PowerShell and Git (x86_64)
- macOS 12+ with Command Line tools (x86_64, arm64)
- Ubuntu 20.04+ with build-essential and Git (x86_64)

Supported in-circuit debuggers (optional but highly recommended):

- [Flipper Zero Wi-Fi Development Board](https://shop.flipperzero.one/products/wifi-devboard)
- ST-Link
- J-Link

Flipper Build System will take care of all the other dependencies.

## Installation

Make sure you have enough space and clone the source code:

```shell
git clone --recursive https://github.com/GuidedJake/GuidedFlipper.git
```

### Building

Build firmware using Flipper Build Tool:

```shell
./fbt
```

### Flashing firmware using an in-circuit debugger

Connect your in-circuit debugger to your Flipper and flash firmware using Flipper Build Tool:

```shell
./fbt flash
```

### Flashing firmware using USB

Make sure your Flipper is on, and your firmware is functioning. Connect your Flipper with a USB cable and flash firmware using Flipper Build Tool:

```shell
./fbt flash_usb
```

## Documentation for Flipper Filmware (might contain information for GudedFlipper Filmware.)

- [Flipper Build Tool](/documentation/fbt.md) - building, flashing, and debugging Flipper software
- [Applications](/documentation/AppsOnSDCard.md), [Application Manifest](/documentation/AppManifests.md) - developing, building, deploying, and debugging Flipper applications
- [Hardware combos and Un-bricking](/documentation/KeyCombo.md) - recovering your Flipper from the most nasty situations
- [Flipper File Formats](/documentation/file_formats) - everything about how Flipper stores your data and how you can work with it
- [Universal Remotes](/documentation/UniversalRemotes.md) - contributing your infrared remote to the universal remote database
- [Firmware Roadmap](/documentation/RoadMap.md)
- And much more in the [documentation](/documentation) folder

# Project structure

- `applications`    - applications and services used in firmware
- `assets`          - assets used by applications and services
- `furi`            - Furi Core: OS-level primitives and helpers
- `debug`           - debug tool: GDB plugins, an SVD file, etc.
- `documentation`   - documentation generation system configs and input files
- `firmware`        - firmware source code
- `lib`             - our and 3rd party libraries, drivers, etc.
- `scripts`         - supplementary scripts and python libraries home

Also, see `ReadMe.md` files inside those directories for further details.

# Links

- Discord: [flipp.dev/discord](https://flipp.dev/discord)
- Website: [flipperzero.one](https://flipperzero.one)
- Forum: [forum.flipperzero.one](https://forum.flipperzero.one/)
- Kickstarter: [kickstarter.com](https://www.kickstarter.com/projects/flipper-devices/flipper-zero-tamagochi-for-hackers)
