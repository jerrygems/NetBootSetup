# Universal PXE Boot Server

[![Mirror & Script Health](https://github.com/jerrygems/NetBootSetup/actions/workflows/health-check.yml/badge.svg)](https://github.com/jerrygems/NetBootSetup/actions/workflows/health-check.yml)

Instantly turn any Linux machine (like a Raspberry Pi or Cloud Server) into a powerful PXE Network Boot Server with a single command.

## Quick Install

Run the following command on the machine you want to turn into a PXE server:

```bash
curl -sL https://boot.jerrygems.tech | sudo bash
```

## Features

- **Dynamic Mirror Querying:** Queries official distro repository mirrors in real-time for full historical version lists.
- **Multi-Distro & Multi-Version:** Install multiple distros and versions concurrently (Linux Mint, Ubuntu, Xubuntu, Kubuntu, Debian Live, Arch Linux).
- **State Detection & Append Mode:** Automatically detects existing PXE setups and non-destructively appends new operating systems without overwriting configurations or re-downloading existing ISOs.
- **16x High-Speed Downloads:** Uses `aria2c` multi-stream acceleration for maximum bandwidth utilization.
- **Production Security:** MAC Address whitelisting and masked Boot Menu Password protection.
- **Universal Compatibility:** Automatically detects server architecture (`x86_64`, `aarch64`, `armv7l`) while serving universal `x86_64` client netboot files.
- **Bulletproof Execution:** Per-command execution verification, ISO corruption detection (<100MB), and safe auto-recovery.
- **Automated Health Monitoring:** Daily GitHub Actions CI/CD pipeline validates mirror reachability and ISO URL resolution without elevated permissions.
- **Clean Uninstall:** Built-in option to cleanly remove the server, delete ISOs, and restore your system.
