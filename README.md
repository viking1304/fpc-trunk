# fpc-trunk

Unofficial macOS binaries for the [Free Pascal Compiler (FPC)](https://www.freepascal.org/) development version (trunk, future 3.3.x).

Built automatically via GitHub Actions (daily) from the latest upstream FPC trunk sources.

Source: [FPC trunk on GitLab](https://gitlab.com/freepascal.org/fpc/source)

Architectures:

- aarch64 (Apple Silicon, M1 and later)
- x86_64 (Intel)

No setup, no compiling. Just download the DMG and install.

[![Build Status](https://github.com/viking1304/fpc-trunk/actions/workflows/build.yml/badge.svg)](https://github.com/viking1304/fpc-trunk/actions/workflows/build.yml)
[![Latest Release](https://img.shields.io/github/v/release/viking1304/fpc-trunk)](../../releases/latest)

## Quick start

1. Go to the [releases](../../releases/latest) page
2. Download the latest DMG for your architecture
3. Open the DMG, double-click the `.pkg` file, follow the installer prompts

Example:

```
fpc-3.3.1-20260419-aarch64-macosx.dmg
```

For official FPC releases visit the [download page](https://www.freepascal.org/download.html).

## What is trunk?

Trunk is the development branch of FPC (future 3.3.x). It includes the latest
features and fixes, but may be unstable.

## Why use this?

- Access the latest FPC features before the official release
- Test compatibility with upcoming versions
- No need to build FPC manually on macOS

## How it works

- Builds run daily
- The workflow pulls the latest FPC trunk source from GitLab
- Each build is tested with a basic hello world program before packaging
- Produces ready-to-use macOS DMG packages for both architectures

## Installation

1. Download the DMG for your architecture
2. Open the DMG
3. Double-click the `.pkg` file inside
4. Follow the installer prompts

The compiler will be installed to `/usr/local/bin`. On Apple Silicon the compiler
binary is `ppca64`, on Intel it is `ppcx64`.

## Naming convention

```
fpc-<version>-<date>-<arch>-macosx.dmg
```

Example:

```
fpc-3.3.1-20260419-aarch64-macosx.dmg
```

## Disclaimer

These are unofficial builds, not official releases from the Free Pascal project,
and come with no guarantees. Use at your own risk, trunk may contain unstable changes.

## License

This repository (build scripts) is licensed under the [MIT License](LICENSE).

Free Pascal Compiler (FPC) is licensed under GPL-2.0-or-later, with RTL and packages under LGPL-2.0-or-later with linking exception.

Each release includes a linked short commit hash and commit title in the release notes.
