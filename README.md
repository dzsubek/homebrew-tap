# dzsubek/homebrew-tap

Homebrew casks by [dzsubek](https://github.com/dzsubek).

| Cask | Description |
| --- | --- |
| `vaultlight` | [VaultLight](https://github.com/dzsubek/VaultLight): a Spotlight-style quick-access panel for your Bitwarden vault on macOS |

VaultLight is an unofficial client and is not affiliated with or endorsed by Bitwarden, Inc.

## Install

Homebrew 6.0 and later only load third-party taps you have explicitly trusted:

```bash
brew tap dzsubek/tap
brew trust --tap dzsubek/tap
brew install --cask dzsubek/tap/vaultlight
```

VaultLight needs macOS 14 or later. The `bitwarden-cli` formula is installed with it.

## Update

```bash
brew upgrade --cask vaultlight
```

## Uninstall

First choose **Lock and Forget** from the VaultLight menu, or **Settings → Sign Out…**. That deletes the stored session key from the Keychain, which `brew` cannot reach. Then:

```bash
brew uninstall --zap --cask vaultlight
```

## How casks get here

Each VaultLight release opens a pull request here that updates `version` and `sha256`. Report problems with the app in [dzsubek/VaultLight](https://github.com/dzsubek/VaultLight/issues).
