# CueGlance — Releases

A native macOS envelope editor for Resolume Arena.

This repository hosts signed, notarized DMG releases of CueGlance.
The source code is private. Bug reports and feature requests are welcome via the [Issues tab](../../issues).

## Download

Latest release: **[Releases page](../../releases/latest)**

All previous versions are available on the [Releases tab](../../releases).

## What it is

Drop in any video — H.264, ProRes, or DXV3 — drag points on the curve, export an XML, apply it on a clip in Resolume. That's the whole loop. Built for VJs who got tired of authoring envelopes inside Resolume's clip inspector and wanted something visual.

The video player is the same one Glance uses, so DXV3 files open and play instantly — same custom GPU decoder, same color accuracy.

## What's in it

- Open any video format Resolume cares about — real DXV3 decoding for the codec you actually deliver shows in
- Scrubbable timeline with cue markers; drop a cue at the playhead with a single keystroke (`c`)
- Interactive envelope canvas — drag points to shape the curve, lock either axis, choose from all 23 Resolume easing types per segment
- Start and End points pinned where Resolume needs them
- Color-cycling cue points so they're easy to tell apart
- Export to Resolume's XML format — drag onto any compatible clip
- Reads existing CueSync `.cueproj` files; saves your own
- Undo, redo, recent files, custom save folder, dark UI that looks like your other VJ tools

## Installing

1. Download the latest `.dmg`
2. Double-click to mount
3. Drag `CueGlance.app` into your Applications folder
4. First launch: macOS verifies the signature and notarization (~2 seconds), then opens

## Requirements

- macOS 14 (Sonoma) or later
- Apple Silicon or Intel Mac
- Resolume Arena 7+ (envelopes export targeted at the 7.23 schema; older Arena versions untested)

## Reporting issues

Please open an [Issue](../../issues) with:

- macOS version (`sw_vers`)
- CueGlance version (visible in the About menu)
- Steps to reproduce
- Screenshot or screen recording if visual

## License

CueGlance binaries are distributed for personal and commercial use.
