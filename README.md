# RollingTail

Tailscale community platforms that actually updates

## Documentation

You can find the documentation for each platform on the [RollingTail website](https://rollingtail.szabee.me/docs).

## Development
This project is currently in currently in beta.

## Platforms
- **Home Assistant**: See the [Home Assistant Documentation](https://rollingtail.szabee.me/docs/platforms/home-assistant) for installation and configuration information.

## How it Works
1. **Renovate** runs on a scheduled basis, scanning Tailscale releases and updating variables across platforms that contain the Tailscale version.
2. For some platforms, a new version number in a config file is enough to trigger an update (aka Tailscale version bump).
