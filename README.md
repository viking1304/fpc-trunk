# fpc-trunk

Unofficial Free Pascal Compiler (FPC) binaries compiled from trunk.

## Why

FPC does not provide official trunk binaries for macOS. This project builds them
automatically from the latest FPC trunk source every day, for both Apple Silicon
(aarch64) and Intel (x86_64).

## Downloads

Get the latest builds from the [releases](../../releases/tag/latest) page.

- `fpc-*-aarch64-macosx.dmg` - Apple Silicon (M1 and later)
- `fpc-*-x86_64-macosx.dmg` - Intel

## Installation

1. Download the DMG for your architecture
2. Open the DMG
3. Double-click the `.pkg` file inside
4. Follow the installer prompts

The compiler will be installed to `/usr/local/bin`. On Apple Silicon the compiler
binary is `ppca64`, on Intel it is `ppcx64`.

## Notes

- Each build is tested with a basic hello world program before packaging
- These are trunk builds, expect occasional breakage
- Not affiliated with the FPC team

## License

The build scripts in this repository are licensed under **MIT** [license](LICENSE).

The distributed binaries are compiled from the
[Free Pascal Compiler (FPC)](https://gitlab.com/freepascal.org/fpc/source) source code.

FPC is licensed under **GPL-2.0-or-later** (compiler) and **LGPL-2.0-or-later** with
linking exception (RTL and packages).

Each release includes the FPC source commit hash in the release notes.
