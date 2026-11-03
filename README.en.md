# ALCASAR Connect 🇬🇧

**by Subaru-Kuzuky** · Windows 10/11 · PowerShell 5.1 · Open source

[Français](README.fr.md) | [Home](README.md)

## Overview

**ALCASAR Connect** is an unofficial Windows tool designed to automate signing in to an **ALCASAR / CoovaChilli** captive portal on networks you are authorized to use.

It features a dark graphical interface, configurable Wi-Fi SSID, editable username and password, a manual connection test, activity logs and a scheduled background connectivity check.

## Features

- Windows graphical interface
- Configurable Wi-Fi SSID and account credentials
- Manual sign-in test
- Scheduled silent checks at Windows sign-in and every two minutes
- Diagnostic activity logs
- Desktop and Start menu shortcuts

## Installation

> **Repository status:** documentation and a sample configuration are available, but the **full application source files have not yet been uploaded**. No verified installable GitHub Release is available yet.

Once the full package is published:

1. Download and fully extract the release archive.
2. Run `INSTALLER.cmd` on Windows.
3. Open **ALCASAR Connect** and enter **your own credentials** and Wi-Fi SSID.
4. Click **Save**, then **Test now**.
5. Refresh the log to inspect the result.

The intended installation directory is `%LOCALAPPDATA%\ALCASAR-AutoLogin`.

## Security and privacy

- **Never commit `config.json`**; it may contain plaintext credentials.
- Use `config.example.json` as a template only.
- Logs may expose network details; review them before sharing.
- Some versions of the legacy authentication engine bypass TLS certificate validation for local portals. This is unsafe on untrusted networks; ask the network administrator to renew expired certificates.
- Use only on networks where you have permission to authenticate. Do not use the tool to bypass network access controls.
- Compatibility depends on the ALCASAR server version and configuration.

## Development and contributions

Issues and contributions are welcome once the complete source code has been published. When reporting a bug, include the app version, Windows version and relevant log lines, **never your password**.

## Credits and license

**Author: Subaru-Kuzuky**

Development assistance: OpenAI ChatGPT.

Independent project; not affiliated with the official ALCASAR team. [MIT License](LICENSE).
