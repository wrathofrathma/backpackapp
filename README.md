# Backpack

> Dual-screen file manager for Android gaming handhelds with full gamepad navigation

A file manager designed specifically for Android gaming handhelds with external display support. Navigate entirely with your controller using a which-key-style hotkey system—no touch required.

<!-- 
![Backpack Screenshot](screenshots/screenshot-1.png)
-->

## Features

- **Dual-pane file management** — Browse files on primary and external displays simultaneously
- **Full gamepad navigation** — Which-key-style hierarchical hotkey menus for discoverable controls
- **Archive support** — Browse, extract, and create ZIP, TAR.GZ, and 7Z archives
- **Background job manager** — Queue long-running operations with progress tracking
- **Favorites & recents** — Quick access to frequently used directories
- **Controller input overlay** — Real-time visualization of button presses
- **Material 3 UI** — Modern Android design with dynamic colors

## Installation

Download the latest APK from the [Releases](https://github.com/wrathofrathma/backpackapp/releases) page.

### Requirements

- Android 13+ (SDK 33)
- Recommended: Gaming handheld with external display support

## Device Compatibility

Designed and tested on Android gaming handhelds:

- Ayn Odin series
- Retroid Pocket series
- Other dual-display capable Android devices

Works on any Android 13+ device, but optimized for controller input.

## Controller Mapping

Navigation uses a which-key-style menu system. Press **X** to open the hotkey overlay, then follow the on-screen prompts.

| Button | Function |
|--------|----------|
| D-Pad | Navigate file list |
| A | Select / Open |
| B | Back / Cancel |
| X | Open hotkey menu |
| Y | Context actions |
| R1/L1 | Switch panes |
| R2/L2 | Page up/down |
| Right Stick | Scroll |
| Start | System menu |
| Select | Toggle input overlay |

### Hotkey Menu Structure

```
X → File operations
    ├─ Clipboard (Copy, Cut, Paste)
    ├─ New (File, Folder)
    └─ Advanced
        ├─ Compression (ZIP, TAR.GZ, 7Z)
        └─ Hash (MD5, SHA256)

X → Search
X → Tabs
X → Selection
X → UI options
X → System
```

## Roadmap

- [ ] FTP server
- [ ] Samba server
- [ ] Cloud storage integration (Google Drive, Dropbox)
- [ ] Root access support
- [ ] Customizable themes
- [ ] Bookmarks & tags
- [ ] Single-screen mode with split pane / tabs
- [ ] Disk space analyzer
- [ ] Touch input support

## About

Source code is maintained in a private repository. Releases are published here.

---

© 2024-2026
