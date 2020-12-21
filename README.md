# samloader_termux

## Introduction

The main purpose why I created this script is being able to download updates for my Galaxy S10+ directly on the device, so that I don't have to download it using Frida on a PC then transfer the AP file to the device, patch it with Magisk and then transfer it back to the PC in order to be able to flash the update using Odin.

## Benefits

- Using the open-source [samloader](https://github.com/nlscc/samloader), so you don't have to rely on

  - closed-source software like Frida

  - Sammobile with their terribly slow download speed

- Don't having to transfer files multiple times across devices

- Don't having to manually deal with samloader's inconvenient syntax

- Automatically install dependencies like python and git

- Option to automatically update samloader to fix download failure

## Installation

1. Download Termux ([Google Play](https://play.google.com/store/apps/details?id=com.termux) or [F-Droid](https://f-droid.org/en/packages/com.termux/))

2. Download this script using `curl -o $PREFIX/bin/samcheck https://raw.githubusercontent.com/lekron42/samloader_termux/main/samcheck`

3. Set executive permissions: `chmod +x $PREFIX/bin/samcheck`

Note: The script offers to install the required dependencies (samloader, python and git) if they are not already installed

## Usage

Just run the script using `samcheck`.
It automatically detects your device model and region.


## Bugs

Most errors should be successfully resolved by updating samloader. Just use `samcheck --repair` for this.

If you still encounter a bug, please create an issue


## Credits and thanks
[nlscc](https://github.com/nlscc) for samloader
