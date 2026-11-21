# CueGlance — Releases

A native macOS envelope editor for Resolume Arena.

This repository hosts signed, notarized DMG releases of CueGlance.
The source code is private. Bug reports and feature requests are welcome via the [Issues tab](../../issues).

## Download

Latest release: **[Releases page](../../releases/latest)** — CueGlance 1.5.2 (fragmented .mp4 files count their real frames), rebuilt in Rust since 1.5.0 (same editor, files and settings as 1.4.1).

All previous versions are available on the [Releases tab](../../releases).

## What it is

Drop in any video — H.264, ProRes, HAP, or DXV3 — drag points on the curve, export an XML, apply it on a clip in Resolume. That's the whole loop. Built for VJs who got tired of authoring envelopes inside Resolume's clip inspector and wanted something visual.

The video player is the same one Glance uses, so DXV and HAP files open and play instantly — same GPU decoders, pixel-exact color.

## What's in it

- Open any video format Resolume cares about — DXV (DXV3, legacy DXV1/2) and every HAP variant on CueGlance's own GPU decoders; H.264, HEVC, ProRes, Motion JPEG and QuickTime Animation through macOS
- Scrubbable timeline with cue markers; drop a cue at the playhead with a single keystroke (`c`)
- Interactive envelope canvas — drag points to shape the curve, lock either axis, choose from all 23 Resolume easing types per segment
- Start and End points pinned where Resolume needs them
- Color-cycling cue points so they're easy to tell apart
- Export to Resolume's XML format — drag onto any compatible clip
- Reads existing CueSync `.cueproj` files and keeps their CueSync fields; saves your own (a project saved by 1.5.0 opens in 1.4.1 and back)
- Undo, redo, recent files, custom save folder, dark UI that looks like your other VJ tools

## Known issues

- Dropping a video can crash CueGlance when the app it was dragged from quits right after the drop (a macOS drag-and-drop bug, reported to Apple; drag from Finder or use File ▸ Load Video… instead). Details: [issue #1](../../issues/1).

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
