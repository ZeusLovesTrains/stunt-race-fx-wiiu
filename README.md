# Stunt Race FX for Wii U (native port), work in progress

An unofficial fan port of the SNES game **Stunt Race FX** to the Wii U (Aroma homebrew, `.wuhb`).
It runs the game natively, built on Jeff's CC0 decompilation, rather than in an emulator.

This game was always a favourite of mine, and it's nice to see it have some great quality of life features that really make it more playable and fair.

> **Work in progress.** It plays well, but there are known rough edges (see below).
> Tested mostly in Cemu, with some testing on a real Wii U.

It's still very much a work in progress, but it plays pretty well, and I figured it would be
fun to have people help me bug-check it. Made with AI, bug-checked with love. Hopefully you
enjoy it! If you find a bug, please [open an issue](../../issues) and let me know.

## Features
- 16:9 widescreen at 720p, including the title screen and menus
- Longer draw distance (adjustable in the pause menu)
- Analog steering, rumble (wall hits, crashes, light buzz on grass)
- Pause menu and `saves/settings.txt`
- Timer at the top right, smaller course map above SPEED
- Resume where you left off (optional)

## Install
1. Download `srfx-native3h-wiiu-noROM.zip` from [Releases](../../releases).
2. Copy its `wiiu` folder to the root of your SD card.
3. Put **your own** ROM in `wiiu/apps/srfx_native3h/` as `srfx.sfc`
   (Stunt Race FX (USA) (Rev 1), CRC32 `380C2635`). No ROM is included.
4. Start "Stunt Race FX native3h" from the Wii U menu.

Pause menu: hold `-` and press `+`, or `ZL+ZR+-`.

**Updating:** your records and best times carry over automatically to each new build.
Only a mid-race resume point is reset when you update.

## Known issues
- Occasional thin gaps or breaks in the road and 3D objects
- A brief 4:3-to-widescreen change before races
- The end-of-race results screen is still 4:3

## Credits
- **Jeff ([jeff-strutb](https://github.com/jeff-strutb/stuntracefx))**: the Stunt Race FX decompilation (CC0). This port builds on it.
- **[Mabec-games](https://github.com/Mabec-games/Stunt-Race-FX-DECOMP)** (CC0): the steady race step and wide-view ideas, reimplemented here.
- devkitPro / wut, SDL2 for Wii U, the Aroma homebrew environment, and Cemu.

Unofficial fan project by ZeusLovesTrains. Not affiliated with or endorsed by Nintendo.
Stunt Race FX is (c) Nintendo. No ROM or Nintendo data is distributed here; you supply your own.
