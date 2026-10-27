# Anti-Alien — Level 6

[English](README.md) · [简体中文](README.zh-CN.md)

**A sci-fi Unreal Engine team game combining research-facility exploration, a desert exterior, gravity changes and a rocket-launch ending.**

This portfolio presents my contribution to **Level 6** of Warwick's WM9M5 team project: audio design and Blueprint implementation, exterior and rocket-area level work, supporting UI, and small-group coordination.

![Exterior layout in the Unreal Engine editor](docs/images/exterior-layout.png)

*Exterior layout from the original project records. The game and environment use team contributions and third-party assets.*

| Context | Details |
| --- | --- |
| Original project | April–May 2026 · University of Warwick · WM9M5 |
| Collaboration | 42-person overall project; I coordinated a group of six |
| Main tools | Unreal Engine 5.4 · Blueprints · Sound Cues · UMG |
| My focus | Audio implementation, exterior layout, rocket-area level work, UI and group coordination |

## My contribution

- **Reusable Blueprint audio:** refactored `BP-MusicManager` for controlled music switching and fades; created `BFL-AudioHelper` with reusable 2D and positional sound calls.
- **Sound connected to play:** worked on desert ambience, interaction and UI feedback, launch audio, attenuation, event debugging and mix balance.
- **Exterior and ending support:** contributed terrain editing, exterior layout and rocket-area level design, connecting the final objective with audio and UI feedback.
- **Supporting UMG UI:** contributed the control guidance, objective information and pause-menu interface.
- **Six-person group coordination:** handled task allocation, progress tracking, meetings and final integration within the wider team project.

These responsibilities describe my contribution to a collaborative game. Other team members and third-party creators contributed gameplay systems, environments and assets.

## Implementation evidence

| System | Purpose | Evidence |
| --- | --- | --- |
| `BP-MusicManager` | Start-music fade-in; fade-out, sound replacement and fade-in through `SwitchMusic`; a launch-music event | [Original Blueprint screenshot](docs/images/music-manager.png) |
| `BFL-AudioHelper` | `PlaySFX2D` exposes sound, volume and pitch; `PlaySFXAtLocation` also exposes world location | [2D helper](docs/images/audio-helper-2d.png) · [Positional helper](docs/images/audio-helper-positional.png) |

The manager screenshot and individual report document the original implementation. The checked Level6 source export contains `BFL-AudioHelper.uasset`, but the `BP-MusicManager.uasset` file has not yet been located. Screenshot evidence and source-file availability are kept distinct. FMOD was separate basic practice and is not presented as this game's middleware implementation.

## Later Windows packaging work

In October 2026, I revisited the archived project with AI-assisted development support to prepare a Windows package. The maintenance record covers the startup map, local UE/MSVC compatibility, spaceship component attachment and World Partition initialization availability.

The repaired full-project candidate completed packaging. Its runtime log contained no spaceship attachment-failure warnings. The trimmed source repository also compiled its editor module and cooked all **1,627 packages with 0 errors and 3 existing warnings**. These checks establish build and startup evidence; full gameplay and audio acceptance remain a separate task.

The test machine required `-dx11` to avoid an observed DX12 GPU crash. This is a machine-specific compatibility path and may alter rendering features.

## Project scope and credits

Level 6 is the sixth level, not an academic qualification level. Original production dates are April–May 2026; the October packaging work is a later maintenance pass.

This is an educational team prototype. Third-party models, textures, audio and other assets retain their original rights. The portfolio does not claim sole authorship of the complete game or grant a blanket licence over team or third-party work.


[Build and validation notes](docs/BUILD_AND_VALIDATION.md) · [Asset publication review](docs/ASSET_PUBLICATION_REVIEW.md)

The complete source archive remains private pending asset-source publication clearance.
