# Rolling Tail

Tailscale community platforms that actually updates

## Development
This project is currently in currently in beta.

## Platforms
- **Home Assistant**: See the [Home Assistant Add-on README](https://github.com/rollingtail/home-assistant/tree/main/README.md) for installation and configuration information.

## How it Works
1. **Renovate** runs on a scheduled basis, scanning Tailscale releases and updating the root `.env` config (and others depending on the platform).
2. Changes to `.env` trigger a **GitHub Actions release workflow** that rebuilds, validates, commits structural config edits back to the repository, and creates a GitHub Release.
