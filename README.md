# Universal PXE Boot Server

Instantly turn any Linux machine (like a Raspberry Pi or Cloud Server) into a powerful PXE Network Boot Server with a single command.

## Quick Install

Run the following command on the machine you want to turn into a PXE server:

```bash
curl -sL https://boot.jerrygems.tech | sudo bash
```

## Features

- **Interactive Setup:** Choose to serve Linux Mint XFCE, Xubuntu, or Arch Linux.
- **Production Security:** MAC Address whitelisting and Boot Menu Password protection.
- **Universal Compatibility:** Automatically detects architecture (arm64/aarch64/amd64) and network settings.
- **Bulletproof Execution:** Per-command verification, ISO corruption checks, and safe auto-recovery on crashes.
- **Clean Uninstall:** Built-in option to cleanly remove the server, delete ISOs, and restore your system.
