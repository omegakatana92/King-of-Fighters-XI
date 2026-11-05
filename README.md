# The King of Fighters XI — Windows & Steam Deck

The King of Fighters XI — Windows & Steam Deck is an unofficial project focused on bringing the PlayStation 2 version of The King of Fighters XI to Windows and Linux, including Steam Deck, using [ps2-native-recomp](https://github.com/exoteric33/ps2-native-recomp) by exoteric33.

The framework translates the PS2’s main processor code into C++ and compiles it into a native executable, while its runtime handles the remaining PS2 hardware functions.

This repository aims to provide game-specific setup instructions, build scripts, launchers, and platform packaging. Planned distribution targets include a Windows setup package and a Linux AppImage for Steam Deck. Development will focus on controller support, graphics, audio, saving, and reliable launching.

## Current status

The project is experimental. Upstream testing reports that The King of Fighters XI plays well, but complete game compatibility and Steam Deck performance require further testing.

This repository currently contains project documentation; working builds and downloads are not yet provided.

## Your own game

Users must supply a disc image from their own copy of the game and generate game-specific files locally. Public packages are intended to contain setup tools and supporting code only, without game assets or translated game code.

## Credits

Credit goes to [exoteric33](https://github.com/exoteric33/ps2-native-recomp) for ps2-native-recomp and [Samir Nuri](https://github.com/snuri00/ps2-web-recomp) for its foundation, ps2-web-recomp. Applicable upstream licenses and copyright notices must be preserved.

This project is not affiliated with or endorsed by SNK or Sony.

## Release description

See [RELEASE_NOTES.md](RELEASE_NOTES.md) for the initial experimental release description draft.

## Short repository description

Experimental Windows and Steam Deck recompilation project for the PS2 version of The King of Fighters XI, using ps2-native-recomp. Requires your own game disc image.
