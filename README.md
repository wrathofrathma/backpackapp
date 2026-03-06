# Backpack

> Dual-screen file manager for Android gaming handhelds, built for full gamepad navigation

A file manager designed for dual screen handhelds with controller input as a first class citizen. 
Inspired by `which-key`, I replaced most touch inputs with key-chords with a visual hotkey overlay.

Single-screen support will come as one of the next major refactors, since I can imagine most single screen
gaming handhelds, or docked devices still could use controller-first file management.

## What is which-key?
`which-key` is a plugin in the editor ecosystem (neovim, emacs, etc), where most actions are exposed
through **key-chords**. Key-chords are simple a sequence of keys, that provoke some functionality to
be triggered. Which makes it perfect for controller-input where we have limited keys to map to many 
functions.

One of the major features of this experience, is also that these key-chords are discoverable due to a
pop-up menu that shows what each button does, and pressing a button takes us to another menu or runs an 
action.

In Backpack, you start a chord with `Y`, then choose from the next layer shown in the overlay.

Examples:

- `Y -> File -> New -> New Folder`
- `Y -> File -> Advanced -> Compression -> Compress ZIP`
- `Y -> File -> Advanced -> Hash -> SHA256 Sum`
- `Y -> UI -> Swap Screens`
- `Y -> Selection -> Select All`

## Demo

- YouTube Short (Prerelease v0.1.0): https://www.youtube.com/shorts/DgoBEA4VJ3I

### Screenshots

<p align="center">
  <img src="screenshots/screenshot-01.png" width="32%" />
  <img src="screenshots/screenshot-02.png" width="32%" />
  <img src="screenshots/screenshot-03.png" width="32%" />
</p>
<p align="center">
  <img src="screenshots/screenshot-04.png" width="32%" />
  <img src="screenshots/screenshot-05.png" width="32%" />
  <img src="screenshots/screenshot-06.png" width="32%" />
</p>

<!-- 
![Backpack Screenshot](screenshots/screenshot-1.png)
-->

## Features

- **Dual-pane file management**: Browse files on primary and external displays at the same time
- **Full gamepad navigation**: Which-key-style hotkey menus to fully replace the need for touch.
- **Archive support**: Browse, extract, and create ZIP, TAR.GZ, and 7Z archives
- **Background job manager**: Queue long operations and track progress
- **Favorites and recents**: Quick access to directories you use often
- **Scoped Storage**: Find and access local storage files for your applications.

## Installation

Download the latest APK from the [Releases](https://github.com/wrathofrathma/backpackapp/releases) page.

You can also use [Obtainium](https://github.com/ImranR98/Obtainium) for update tracking:

- Add this repo URL: `https://github.com/wrathofrathma/backpackapp`
- Enable **Include pre-releases** in Obtainium so alpha builds are detected

### Requirements

- Android 13+ (SDK 33)
- Recommended: Gaming handheld with external display support

## Device Compatibility

Built and tested on the **Ayn Thor**.

Other Android 13+ dual-screen devices may work too but no promises yet.

## Controller Mapping

These are the base key-shortcuts available outside of the primary hotkey menu.

| Button | Function |
|--------|----------|
| D-Pad | Navigate file list |
| Left Stick | D-Pad navigation |
| A | Select / Open |
| B | Back / Cancel |
| X | Open favorites |
| Y | Open hotkey menu |
| L1 | Page up |
| R1 | Page down |
| L2 | Open Applications (App Storage) |
| R2 | Open Recents |
| Right Stick (directional) | Change focused screen |
| R3 (Right Stick Click) | Swap screens |
| Start | System menu |
| Select | Multi-select |

### Key-chords / hotkey menu
Everything else is accessed via **key-chords**, starting with **Y**.

```
Y → Main Layer
    X  → File
    R1 → UI
    Start → Open
    Select → Selection
    R2 → Refresh
    L2 → Favorite

Y → File Layer
    X  → Move
    Y  → Clipboard
    L1 → Delete
    R1 → Rename
    Start → Advanced
    Select → Share
    R2 → New
    L2 → Properties

Y → File → Clipboard
    X → Copy

Y → File → New
    X → New File
    Y → New Folder

Y → File → Advanced
    X  → Compression
    L1 → Hash
    R1 → Duplicate

Y → File → Advanced → Compression
    X  → Compress ZIP
    Y  → Compress TAR.GZ
    L1 → Compress 7Z
    R1 → Decompress Here
    Start → Decompress To...

Y → File → Advanced → Hash
    X  → SHA256 Sum
    Y  → MD5 Sum
    L1 → Compare SHA256
    R1 → Compare MD5

Y → UI
    R2 → Toggle Input Overlay (off by default)
    L2 → Swap Screens

Y → Selection
    X  → Select Mode
    Y  → Clear Selection
    L1 → Select All
    R1 → Invert Selection

Y → Open
    X  → Favorites
    Y  → Recents
    L2 → Applications
    R2 → Job Manager
```

## Roadmap

Rough roadmap for now:

- [ ] FTP server (target: v1.0)
- [ ] Disk space analyzer (target: v1.5)
- [ ] Single-screen mode with split pane / tabs (target: v2.0)
- [ ] Touch input support (target: v2.5)
- [ ] Cloud storage integration (Google Drive, Dropbox) (target: v3.0)
- [ ] Root access support (target: v3.0)
- [ ] Customizable themes (target: v3.5)
- [ ] Samba server (target: TBD)

## About

Source code is maintained in a private repository. Public releases are published here.
