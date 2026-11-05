# The King of Fighters XI — v0.1.0-beta (release candidate)

> Release notes prepared for a beta release. The GitHub release and binary assets have **not yet been published**.

Experimental native Linux / Steam Deck runner for the PlayStation 2 version of **The King of Fighters XI (Europe, SLES_544.37)**, using [ps2-native-recomp](https://github.com/exoteric33/ps2-native-recomp).

## Verified on the developer's Steam Deck

- Native Linux runner launches the game.
- Steam Deck AppImage launches with the supplied game files.
- Graphics, audio and Steam Deck controller work in local testing.
- Memory card is detected and an existing save was read.
- Updated AppImage includes SDL2 and passed a roughly 33-second local launch test with zero audio underruns.
- A separate test using invalid compiler environment overrides also launched successfully, but this **does not establish compiler independence**, because fallback compilers and existing translation caches may still be used.

## Beta limitations

- **Not tested on a clean Steam Deck or another Linux system.** The runtime may still need an external C++ compiler for EE/VU live translation; the developer machine has a separate 2.5 GB toolchain installed.
- Gaming Mode, Windows release binaries, and full-game completion have not been verified.
- The package is experimental, not a guaranteed standalone native recompilation.
- No copyrighted game ISO, ELF, BIOS, extracted assets, or translated game code should be uploaded.

## Planned release assets

- `KOF-XI-Steam-Deck-x86_64.AppImage` (built and locally tested; not yet uploaded)
- `KOF-XI-Steam-Deck-x86_64.AppImage.sha256` (generated locally; not yet uploaded)
- Native Linux archive (pending packaging and verification)

SHA-256 for the locally tested AppImage:

```text
63423e1e52a745e0a65a764c8d63f551808a727690d77f39f5f762c8da026f67  KOF-XI-Steam-Deck-x86_64.AppImage
```

## Local installation / testing

1. Supply your own legally obtained European PS2 game disc image and extracted executable.
2. Place the ISO at `~/.local/share/kof-xi/game/disc.iso` and the executable at `~/.local/share/kof-xi/game/SLES_544.37`.
3. Mark the AppImage executable: `chmod +x KOF-XI-Steam-Deck-x86_64.AppImage`.
4. Run it on a compatible Linux x86-64 system. If FUSE is unavailable, try `./KOF-XI-Steam-Deck-x86_64.AppImage --appimage-extract-and-run`.
5. Save data is stored under `~/.local/share/kof-xi/saves/`.

This is an unofficial community project, not affiliated with SNK or Sony. The King of Fighters XI and related assets belong to their respective rights holders.

## Credits

Built using ps2-native-recomp by exoteric33.
