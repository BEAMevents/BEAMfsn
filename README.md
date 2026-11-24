# BEAMfsn

Turns a Barco FSN **RCP-120** remote panel into a button box for network commands, like Bitfocus Companion: its 12 LCD buttons make routes on a **Riedel MediorNet** router (Ember+) or send TCP, UDP and HTTP commands, with your own labels and colours on the buttons. No FSN switcher needed. By [BEAM Events](https://beamevents.com).

This repository only holds the **installers and updates**.

## Download
Get the latest version from **[Releases](https://github.com/BEAMevents/BEAMfsn/releases/latest)**:

- **BEAMfsn-x.y.z-mac-arm64.dmg** (Mac, Apple Silicon).
- **BEAMfsn-Setup-x.y.z.exe** (Windows) installs BEAMfsn. **BEAMfsn-Portable-x.y.z.exe** runs without installing.

The Mac app is signed and notarized by Apple, so it opens with a normal double-click; allow it to find devices on your local network when macOS asks. The Windows installer isn't code-signed yet, so SmartScreen may warn on first launch: click **More info → Run anyway**, and allow BEAMfsn through Windows Firewall so the panel's button presses can reach it.

## Setting up the panel
On the RCP-120's web page (`http://<panel address>/`) set **Master Controller IP Address** to the computer running BEAMfsn, **Master Controller Port** to `10101` and **Button Release Notify Variable Name** to `beamfsn`, then Update and Reboot. Type the panel's and the MediorNet's addresses into BEAMfsn and click a button to set it up.

## Updates
Click the version number at the top of the window. Installed copies download new versions in the background and show **Update x.y.z ready**: click it, then **Install & restart**. Nothing installs while the panel is in use.

## Problems?
Use **Help → Send Diagnostics to BEAM…** (or the version number at the top). It sends BEAMfsn's log, its button setup and a short status report to BEAM.
