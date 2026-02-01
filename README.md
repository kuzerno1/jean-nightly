# Jean Nightly

Nightly build repository for [Jean](jean/README.md) — an AI assistant application for managing multiple projects, worktrees, and sessions with Claude CLI.

## Repository Structure

| Directory | Description |
|-----------|-------------|
| [`jean/`](jean/) | Main Tauri application (React + Rust) with full documentation |
| [`patches/`](patches/) | Git patches for nightly-specific customizations |
| [`.github/workflows/`](.github/workflows/) | CI/CD workflows for nightly builds |

## Quick Start

See the main application documentation:

- **[README](jean/README.md)** — Features, screenshots, prerequisites
- **[CONTRIBUTING](jean/CONTRIBUTING.md)** — Development setup and guidelines
- **[CLAUDE.md](jean/CLAUDE.md)** — Development guide for AI-assisted coding

## Patches

The `patches/` directory contains modifications applied to the nightly build:

| Patch | Purpose |
|-------|---------|
| `001-disable-macos-signing.patch` | Disable macOS code signing for dev builds |
| `002-update-updater-endpoint.patch` | Point updater to nightly release channel |
| `003-rename-application.patch` | Rename app for nightly distribution |

## CI/CD

The nightly workflow (`.github/workflows/nightly.yml`) builds and publishes releases for:

- macOS (Universal)
- Windows (MSI, NSIS)
- Linux (DEB, RPM, AppImage)

## Contributing

This is a nightly build repository. To contribute to Jean, please visit the main repository:

**[github.com/coollabsio/jean](https://github.com/coollabsio/jean)**

## License

[Apache 2.0](jean/LICENSE.md)

---

All credits go to [Andras Bacsai](https://x.com/heyandras) and the [coolLabs](https://coollabs.io) team.
