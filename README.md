# Unofficial Native Runtime for Sega 32X Virtua Racing Deluxe (AOT Recompiler)

**No ROM or assets included.**

An unofficial native runtime and AOT recompiler compatible with the retail Sega 32X *Virtua Racing Deluxe* cartridge.

Features enhanced 16:9 widescreen presentation, 60 FPS, antialiasing, dynamic lighting, and native execution on modern PC systems.

> [!NOTE]
> Not affiliated with, endorsed by, or sponsored by SEGA. See [`NOTICE`](NOTICE).

---

## Requirements

**This repository contains no copyrighted game files, ROMs, or proprietary assets.**

To play, you must supply your own legally acquired dump of the retail *Virtua Racing Deluxe* (Sega 32X) cartridge:

- Place your ROM dump in the `rom/` folder (`.32x` or `.bin`).
- Supported cartridge: North American release (`MK-84601`, revision `00`, region `U`).
- Verification hash (SHA-256): `cc2917895842ba42ce871a07a327c5467a5b5df8b7999ccc4b7b5bea9d4caf6b` (3,145,728 bytes).

---

## How to Play

1. Download the latest release `.zip` for Windows or Linux from the **[Releases](https://github.com/s32xfan/virtuaracing/releases)** page.
2. Extract the `.zip` archive.
3. Put your legally owned ROM dump inside the `rom/` folder.
4. Launch the game:
   - **Windows:** Double-click `vr32x-native.exe`
   - **Linux:** Run `./vr32x-native`

No compiler, runtime dependencies, or external emulators required.

---

## Controls & In-Game Settings

| Action | Keyboard | Gamepad |
|---|---|---|
| Steering / Throttle | Arrows / WASD | D-pad / Left Stick |
| Accelerate | Ctrl / Z | A |
| Brake | Alt / X | B |
| Change View | Space | X / C |
| Start | Enter | Start |
| **Settings Menu** | **Esc** | Guide / Back |

### Configuration Menu
- Press **`Esc`** at any time during gameplay or title screen to open/close the in-game Settings.
- Use **Up/Down** to navigate and **Left/Right** to adjust values.
- **Visual Presets:** Choose from *Original*, *Performance*, *Balanced*, *Quality*, or *Ultra*.
- **Custom Graphics:** Customize widescreen presentation, antialiasing, draw distance, and ambient occlusion. Changes take effect immediately.

---

## License

This project is licensed under the MIT License — see [`LICENSE`](LICENSE) and [`NOTICE`](NOTICE).
Third-party software licenses are documented in [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md).
