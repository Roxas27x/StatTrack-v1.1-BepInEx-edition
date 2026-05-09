# BepInEx Plugins for Clone Hero v1.1

Runtime BepInEx 6 IL2CPP plugins for Clone Hero v1.1.

These packages do not patch or replace Clone Hero game binaries. Plugins are loaded by BepInEx at runtime from `BepInEx/plugins`.

## Install

Download `BepinexV1.1.zip` and extract it into the root of your Clone Hero v1.1 folder, the same folder that contains `Clone Hero.exe`.

This main package includes BepInEx 6 IL2CPP x64. After extraction, launch Clone Hero. The first launch may take longer while BepInEx generates IL2CPP interop files.

Download the additional `.zip` files as desired and extract them into the same Clone Hero v1.1 folder. Let the folders merge when prompted.

**NOTE: Use DX11 rendering API for the best results. DX12 / Vulkan induces stutter/lag issues, and they are generally less stable than DX11.**

## Downloads

### `BepinexV1.1.zip`

Required base package. Installs BepInEx 6 IL2CPP x64 for Clone Hero v1.1.

Install this first before adding any plugin zips. This package does not include gameplay plugins by itself.

### `NoteSplitv11.zip`

Adds NoteSplit support for Clone Hero v1.1.

This tracks section-by-section miss counts, personal bests, previous run data, song speed and difficulty variants, and opens a separate NoteSplit overlay window that can be positioned or captured externally.

### `AdaptivePracticeV11.zip`

Adds Adaptive Practice mode for Clone Hero v1.1 practice mode.

When practicing a section, the chart waits at each note or chord group and advances after Clone Hero accepts the hit. It uses your selected practice speed, keeps audio synced while notes are moving, and helps practice difficult sections without notes flying past before you are ready.

### `StatTrackSectionAnalytics.zip`

Adds section analytics for Clone Hero v1.1.

This tracks section consistency, section performance history, and FC chance style analytics so you can review which parts of a chart are improving or causing breaks.

## Safety

This release does not patch `Clone Hero.exe`, `GameAssembly.dll`, or game data files.

Plugins are loaded through BepInEx at runtime. To remove a plugin, delete its folder from `BepInEx/plugins`.

## Troubleshooting

If BepInEx or a plugin does not load:

1. Confirm the files were extracted into the folder containing `Clone Hero.exe`.
2. Confirm the plugin DLL exists under `BepInEx/plugins/<PluginName>/`.
3. Launch the game once and check `BepInEx/LogOutput.log`.
4. If the first launch takes a while, wait for BepInEx IL2CPP interop generation to finish.

## Third-Party Software

`BepinexV1.1.zip` bundles BepInEx and .NET runtime components required by the loader. See `THIRD_PARTY_NOTICES.txt` for attribution and license notes.
