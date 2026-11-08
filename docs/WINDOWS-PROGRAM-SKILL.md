# Windows Program Skill

This repository documents the reusable Windows executable standard. The distributable ChatGPT skill is packaged separately as `skill.zip` for installation.

## Trigger
Whenever asked to make a Windows program, desktop GUI, native dashboard, installer, or portable executable.

## Required deliverable
- Compiled 64-bit Windows GUI `.exe` as the main artifact; do not substitute .bat, PowerShell, Python, a web shortcut or source archive.
- Proper app-specific embedded icon set on title bar, taskbar and Alt+Tab.
- Bottom-right compact small N8 mark, `Install Updates` control and truthful update status.
- Use verified HTTPS release manifests, semantic version comparison and signed/checksum verified binary before installation. Never run an arbitrary URL from an untrusted response.
- Native GUI must launch without manual runtime setup; preserve working features.
- Validate executable PE type, imports, resources and run on actual Windows where available.
- Distinguish built functions from stubs, untested features and missing external credentials.
- Optional source package is not a substitute for compiled executable.

## Mount Olympus implementation
This project's current GUI executable is a standalone dashboard shell. Its Windows build and icon resources are present, but cloud hosting, provider integrations and fully automated verified installation require further implementation. See [Platform Requirements](PLATFORM-REQUIREMENTS.md).
