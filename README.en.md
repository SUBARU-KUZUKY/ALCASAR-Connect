# ALCASAR Connect 🇬🇧

**by Subaru-Kuzuky** · Windows 10/11 · PowerShell 5.1 · MIT License

[Français](README.fr.md) | [Home](README.md)

## Overview
Unofficial Windows app for automatic sign-in to ALCASAR / CoovaChilli captive portals on authorized networks. Dark graphical interface, configurable Wi-Fi, editable credentials, manual testing, silent scheduled login, and connection logs.

## Installation and testing
Documentation is online, but **the full source code and downloadable Release have not yet been uploaded to GitHub**. The testing package may be used locally meanwhile.

1. Extract the full package.
2. Run `INSTALLER.cmd` on Windows.
3. Enter the Wi-Fi SSID and **your own credentials**; select **Save**.
4. Test the connection and use **Refresh** to read the log.

The intended installation directory is `%LOCALAPPDATA%\ALCASAR-AutoLogin`. Scheduled checks can run every two minutes.

## Security
Never publish `config.json`, passwords, or logs containing private information. The current engine disables certificate checks on local TLS requests: use only on a trusted network while the administrator fixes certificate problems. This is an unofficial tool and compatibility depends on the portal version. Use only where you have permission.

## Credits
**Developed by Subaru-Kuzuky** · Technical assistance: **OpenAI**.

[MIT License](LICENSE). Contributions welcome once full sources are published.
