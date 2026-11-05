# Appman

**A terminal-based Android application manager for rooted devices.**

Appman provides an interactive interface for browsing installed applications, switching between Android users and profiles, inspecting package information, and managing application states.

## Features

- Dynamic Android user and profile discovery.
- Secure Folder and work profile support where compatible.
- User-installed and system application views.
- Interactive package selection.
- Freeze, enable, and per-user uninstall operations.
- Live package preview and disabled-state indicators.
- Search, keyboard navigation, and clickable header tabs.

## Requirements

- Android with root access.
- Termux and fzf.
- Working root-capable sudo command.
- aapt2 (optional, for application labels).

## Installation

```sh
git clone https://github.com/royalewhite/Appman.git
cd Appman
chmod 755 appman appman-preview appman-profiles
./appman
```

## Keyboard controls

| Key | Action |
|---|---|
| ALT-1 to ALT-9 | Switch profiles |
| Header click | Switch profile or filter |
| ALT-U | User apps |
| ALT-Y | System apps |
| SPACE | Select / deselect |
| U | Clear selections |
| ENTER | Uninstall selected apps |
| CTRL-F | Freeze selected apps |
| CTRL-T | Enable selected apps |
| CTRL-R | Toggle search |
| ESC | Clear search |
| ? | Help |
| CTRL-Q | Quit |

## Safety

- Actions target only the active Android user.
- Batch uninstall requires confirmation.
- Profile changes clear selections.
- No select-all shortcut is provided.
- Per-user uninstall does not necessarily remove the underlying system APK.

## Compatibility

Tested on Samsung Galaxy M14 5G, Android 15 / One UI 7, with Termux and root. Other devices and profile implementations may vary.

## Contributions

Bug reports, compatibility reports, and feature suggestions are welcome through GitHub Issues.
