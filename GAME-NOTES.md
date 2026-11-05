# Game Notes and License Information

## Project status

This repository is the GPL source release for Doom 3. It is the engine source code and project files, not a complete packaged build of the game.

## Important usage notes

From the project README:

- the game data is not included in this source release
- the data remains covered by the original EULA
- a patch to the latest game version is required
- the project is for engine development and modification

## Build and platform notes

The README points users to:

- Visual Studio 2010 project files on Windows
- SCons on GNU/Linux
- Xcode 3.2 on macOS

The source tree also includes platform-specific support for Windows, Linux, and Mac OS X.

## Licensing

The primary license is the GNU General Public License, as described in `COPYING.txt`.

The README also notes that Doom 3 GPL source code is subject to additional terms beyond the GPL. The exact wording in `README.txt` should be read before distribution or redistribution.

## Third-party code contained in the tree

The project contains third-party dependencies and bundled libraries, including:

- cURL
- JPEG library code
- OggVorbis
- PropTree
- OpenAL SDK

These are documented in the licensing sections of `README.txt` and are provided with their own notices and permissions.

## Suggested starting points

If you are exploring the engine, good starting points are:

- `neo/idlib/` for the engine core and foundational systems
- `neo/framework/` for engine infrastructure
- `neo/game/` for game-specific logic
- `neo/renderer/` for rendering and graphics work
- `neo/sound/` for audio systems

This repository is a classic engine source tree, so it is best approached by understanding the build scripts and the major subsystems before editing gameplay code.
