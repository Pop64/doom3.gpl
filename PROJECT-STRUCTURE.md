# Project Structure

The repository is divided into a small top-level set of distribution files and a large `neo/` engine tree that contains the actual source code and build configuration.

## Top-level files

- `README.txt` — project overview, build instructions, and licensing notes
- `COPYING.txt` — GPL license text
- `.gitignore` — ignores local build output
- `base/` — game data directory expected to be supplied separately
- `neo/` — engine, tools, renderer, scripts, and project files

## Engine tree (`neo/`)

The major directory layout is as follows:

```text
neo/
├── cm/            core math / collision / model code
├── curl/          bundled cURL source
├── d3xp/          Doom 3 expansion content and logic
├── framework/     base engine framework and subsystems
├── game/          game-specific logic and content hooks
├── idlib/         id Software's core library
├── MayaImport/    Maya importer plugin source
├── openal/        OpenAL SDK files and wrappers
├── renderer/      rendering system and drivers
├── sound/         audio system and bundled dependencies
├── sys/           platform-specific system code
├── tools/         tools and utilities used by the engine
├── ui/            UI-related source
├── TypeInfo/      type info generation/mapping support
├── SConstruct     SCons build entry
├── doom.sln       Windows Visual Studio solution
├── *.vcxproj      Visual Studio project files
├── run.bat        Windows run script
├── clean.bat      Windows cleanup script
└── ...            additional build and support files
```

## Runtime data note

The repository intentionally omits the actual game assets. The `base/` directory is present as a placeholder for data, but the original game data is not distributed in this source release. You must use the original licensed game files and apply the required patches to match the engine version.
