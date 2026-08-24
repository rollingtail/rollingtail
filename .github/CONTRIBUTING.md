# Contributing to Rolling Tale

Thank you for your interest in contributing to Rolling Tale! This project aims to keep Tailscale community packaging continuously updated and robust.

## How to Contribute

### 1. General Guidelines
- Do not manually update versions in `.env` or configuration files unless you are testing a specific release issue. The system is designed to have **Renovate** update versions on a schedule.
- If you want to configure build steps or add support for another platform, open a Pull Request describing your changes.

### 2. Local Development & Testing
If you modify the Home Assistant addon files, you should verify they compile successfully by running Docker locally before submitting:
```bash
 docker build --build-arg TAILSCALE_VERSION=1.102.3 --build-arg BUILD_ARCH=amd64 -t test-tailscale tailscale
```

### 3. Submission Process
1. Fork the repository and create your branch from `main`.
2. Make your code changes and verify they compile/build cleanly.
3. Submit a Pull Request targeting the `main` branch.
4. Ensure your PR description templates are filled out.
