# reDivert

**reDivert** is a Windows split-tunneling utility for VPN configurations that use a real tunnel network adapter.

The program allows you to keep VPN enabled for the whole system while giving selected applications direct network access through the normal home connection.

## What reDivert is for

reDivert is designed for situations where VPN should remain active for the entire PC, while specific applications need to work through the regular local connection.

This is useful when part of your software should stay on VPN and part should connect directly, without manually switching the whole system back and forth.

## How it works

The user selects the normal home adapter, then the active VPN adapter, adds the required applications, and applies the configuration. After that, the selected programs work directly, while the rest of the system continues to use VPN.

## Key features

- split tunneling for selected applications;
- VPN remains active for the whole system by default;
- Russian and English interface support;
- designed for VPN scenarios with a real Windows tunnel adapter;
- simple and clear interface without unnecessary complexity.

## Supported VPN scenarios

reDivert is designed for VPN environments where Windows creates a real tunnel network adapter.

Confirmed scenarios:

- RedVPN
- Outline
- v2RayTun in Sing-box + Tunnel mode

## Important notes

- administrator rights are required for normal operation;
- the program is intended for supported VPN scenarios with a tunnel adapter;
- packet contents are not logged;
- reDivert is a local routing utility and is not intended for traffic content analysis, hidden interception, or similar use cases.

## Third-party component

reDivert uses **WinDivert** as a third-party networking component.

Special thanks to **basil** and the **WinDivert** project for the technical foundation that made this routing model possible.

More details are available in `README_Technical.md`, `THIRD_PARTY_NOTICES.txt`, and the included third-party license texts.

## Technical information

Detailed technical information and usage instructions: [README_Technical.md](README_Technical.md)