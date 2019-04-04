# Rojo for VS Code

This is a VS Code extension that gives you [Rojo](https://github.com/LPGhatguy/rojo) automatic installation and integration.

Works on both Windows and macOS.

## How to use

- **If you are a new user**, please open the command panel (`Ctrl+Shift+P`) and run `Rojo: Open welcome screen` to see a guide.
- Otherwise, the extension will automatically activate whenever you have a `rojo.json` file in the root of your workspace or when you run a Rojo command.

## Features

- Automatically downloads the latest version of Rojo and keeps you up to date.
- Can automatically install the Roblox Studio plugin as well.
- Start and stop Rojo in one click, no need to touch the command line.
- Generates (and provides schema helpers for) rojo.json.
- Includes a quick start guide to help new users get started (`Rojo: Open welcome screen`)

## Requirements

- Windows, or
- macOS with [cargo installed](https://doc.rust-lang.org/cargo/getting-started/installation.html)

## Acknowledgements

- [LPGhatguy](https://github.com/LPGhatguy), for creating and maintaining Rojo.

## Known Issues

- None yet

## Release Notes

### 1.5.0

- Add Rojo build command
- Add convert from rojo.json to default.project.json

### 1.4.0

- Rojo v0.5.x is now supported! Check out [this page](https://lpghatguy.github.io/rojo/migrating-to-epiphany/) for details on how to migrate your project.
- To enable automatic pre-release downloads, open the extension settings panel and select the "pre-release" release type. Note: VS Code may need to be reloaded after this change.
- You can now target a specific Rojo version instead of the latest. Change the targetVersion setting to the tag name of the release you want to install (for example, v0.4.13). You can change this at the workspace level to lock projects to specific Rojo versions for compatibility.
- The "Rojo: Create Partition Here" context menu entry is now "Sync from here" and is compatible with both Rojo v0.4.x and v0.5.x.

### 1.3.0

- macOS support thanks to a PR from [Anton Matosov](https://github.com/anton-matosov).

### 1.2.5

- Added "Rojo: Create partition here..." context menu entry when right-clicking files or folders in the explorer.

### 1.2.1 - 1.2.4

- Adjusted welcome screen guide contents.

### 1.2.0

- Added new welcome screen with quick-start guide.
  - Forces users to pick if they want to manage the plugin, or if they want the extension to.
- Added plugin management and installation.
  - New setting `rojo.robloxStudioPluginsPath` if you have a weird plugins folder (default should be correct for 99% of people)/
- Added event logging to help track down any loose bugs that are encountered in the wild and for automatic detection of an invalid release.
  - Opt-out with `rojo.enableTelemetry` set to `false`.
- General code restructuring and improvements under the hood.

### 1.0.0

Initial release of vscode-rojo
