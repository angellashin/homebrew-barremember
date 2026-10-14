# Homebrew BarRemember

Homebrew Cask for [BarRemember](https://github.com/angellashin/Bar-Remember),
a native macOS menu bar companion for Apple Reminders.

## Install

```sh
brew tap angellashin/barremember
brew install --cask barremember
```

This Cask supports Apple Silicon Macs running macOS 14 Sonoma or later.

Recent Homebrew versions require an explicit local trust decision before loading
a third-party Cask. Review this public tap first; if you choose to trust it, run
`brew trust angellashin/barremember` before the install command. This stores a
local Homebrew trust setting and is not performed by BarRemember.

## Security status

The current app is ad-hoc signed and is not Developer ID signed or
Apple-notarized. Gatekeeper can therefore warn about or block the first launch.
Do not weaken macOS security protections or remove quarantine attributes to run
it. A signed and notarized release requires Apple Developer Program membership.

## Update

```sh
brew update
brew upgrade --cask barremember
```

## Maintainer release steps

1. Build and validate a versioned ZIP from the source repository.
2. Publish the ZIP and its SHA-256 to the matching GitHub Release first.
3. Update this Cask's `version`, URL, and `sha256` to exactly match that asset.
4. Run Homebrew Cask style and audit checks, then commit and push this tap.
