# reDivert — Technical Information

## Purpose

**reDivert** is a Windows split-tunneling utility for VPN configurations that use a real tunnel network adapter.

The program allows you to keep VPN enabled for the whole system while routing selected applications directly through the normal home connection.

## Supported operating model

reDivert is designed for scenarios where the VPN client creates a separate tunnel adapter in Windows.

Confirmed scenarios:

- RedVPN
- Outline
- v2RayTun in Sing-box + Tunnel mode

## Requirements

For normal operation, the following are required:

- Windows;
- administrator rights;
- an active VPN that creates a real tunnel network adapter.

Without administrator rights, the program cannot operate in normal mode.

## Quick start

1. Run **reDivert.exe** as administrator.
2. In the **Интернет** section, select the normal home adapter.
3. In the **VPN** section, select the active VPN adapter.
4. Add one or more applications to the routing list.
5. Click **Применить**.
6. Click **Старт**.
7. Make sure the selected applications use the normal home connection while the rest of the system continues to work through VPN.

To stop routing, click **Стоп**.

## Important notes

- the program is intended for supported VPN scenarios with a tunnel adapter;
- the interface is available in Russian and English;
- the release uses one built-in **WinDivert 2.2.2 (variant A)** path;
- packet contents are not logged;
- reDivert is a local routing utility and is not intended for traffic content analysis, hidden interception, or similar use cases.

## What is not supported

The program is not designed for the following modes or scenarios:

- VPN solutions that operate only in proxy-only mode;
- routing models outside the “home adapter + VPN adapter” scheme;
- hidden operation, masking, or bypass of protection mechanisms;
- capture of packet contents;
- use cases related to anti-cheat bypass.

## Logs and working data

The program stores its working data in:

`%USERPROFILE%\Desktop\reDivert`

The log file is located at:

`%USERPROFILE%\Desktop\reDivert\logs\reDivert.log`

The log contains:

- startup and shutdown events;
- routing state changes;
- diagnostic information;
- runtime errors.

Packet contents are not written to the log.

## Third-party component: WinDivert

reDivert uses **WinDivert** as a third-party networking component.

WinDivert is developed by **basil** and distributed under its own license terms. Details are provided in `THIRD_PARTY_NOTICES.txt` and in the `third_party_licenses` directory.

This release uses **WinDivert 2.2.2 (variant A)**.  
The source code for this version is included with the release.

Official project pages:

- [WinDivert on GitHub](https://github.com/basil00/WinDivert)
- [WinDivert documentation](https://reqrypt.org/windivert-doc.html)

## Public release contents

The public release includes:

- `reDivert.exe`
- `README.md`
- `README_EN.md`
- `README_Technical.md`
- `README_Technical_EN.md`
- `THIRD_PARTY_NOTICES.txt`
- `LICENSE`
- third-party license files (`GPL-2.0.txt` and `LGPL-3.0.txt`)
- the source archive for the WinDivert version used in the release

---

<details>
<summary><b>Русская версия (нажмите, чтобы открыть)</b></summary>

<br>

Техническая документация на русском языке: [README_Technical.md](README_Technical.md)

</details>