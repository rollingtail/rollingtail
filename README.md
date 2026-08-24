# Rolling Tale

Tailscale community platforms that actually update

This repository contains third-party community packaging of Tailscale (e.g., Home Assistant addons) that are automatically tracked and updated using Renovate workflows.

## Development

This project is currently in currently in beta.

## Platforms
- **Home Assistant**: See the [Home Assistant Add-on README](platforms/home-assistant/README.md) for installation and configuration information.

## How it Works
1. **Renovate** runs on a scheduled basis, scanning Tailscale releases and updating the root `.env` config.
2. Changes to `.env` trigger a **GitHub Actions release workflow** that rebuilds, validates, commits structural config edits back to the repository, and creates a GitHub Release.
