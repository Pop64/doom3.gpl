# Building Doom 3 GPL

This project is the original GPL source release for Doom 3. The source tree is under `neo/`, and the build instructions in the project README are the most authoritative reference.

## Requirements

- A working C++ toolchain
- Microsoft Visual Studio 2010 for Windows builds
- DirectX SDK for Win32 builds
- SCons for GNU/Linux builds
- Xcode 3.2 for the Mac OS X project under `neo/sys/osx/`

## Windows build

Use the Visual Studio solution in:

```text
neo/doom.sln
```

The README notes that Microsoft Visual Studio 2010 Express cannot build the project successfully because 32-bit MFC support is required, and the DirectX SDK is also needed.

## Linux build

From the `neo/` folder, run:

```bash
scons
```

The project documentation states that the GNU/Linux build uses SCons.

## macOS build

The project includes an Xcode 3.2 project under:

```text
neo/sys/osx/
```

## Important notes

- This source release does not include the game data files.
- You must patch the game to the latest version before running a build.
- The game data remains under the original EULA and license terms.
- This repository is a source tree for the engine, not a full standalone game package.
