# Anti-Alien Level6

Unreal Engine 5.4 game project. Entry map: `/Game/LEVEL-6`.

## Branches

- `main`: source baseline before the Windows packaging fixes.
- `codex/level6-packaging-fix`: the packaged and tested candidate; use this branch for the current version.

## Open the project

Install Unreal Engine 5.4.4, Git LFS, and the Visual Studio C++ game-development toolchain. Clone the repository, switch to `codex/level6-packaging-fix`, run `git lfs pull`, then open `Level6.uproject`. Open `Content/LEVEL-6.umap` in the editor.

Binary Unreal assets are stored in Git LFS. A GitHub ZIP download may contain LFS pointers; clone with Git LFS to retrieve the assets.

## Source scope

This repository contains the LEVEL-6 cooked package source counterparts, local dependencies discovered through the source Asset Registry, and the game's custom gameplay/audio/UI assets. The manifest lists the included packages. Unused vendor demos, the Developers folder, generated caches, editor binaries, and packaged Windows builds remain outside Git. The complete local asset library is preserved separately.

Three legacy references already have no corresponding source package in the local project: `SKM_Manny`, `SKM_Quinn`, and the FirstPersonArms `SKM_Mannequin`. The tested Windows package cooked successfully with these existing references; this repository does not invent replacements.

## Validation

The packaging-fix candidate completed Windows packaging. Its runtime log contained no spaceship attachment-failure warnings. The user reported that the newly opened candidate appeared correct; complete shooting, jumping, audio, and full-gameplay acceptance has not been independently established.

The local DX12 build produced a GPU crash on the test machine. Use `-dx11` when launching the Windows executable on that machine. DirectX 11 can change rendering features.

## Assets

Third-party asset rights remain with their respective owners. No blanket open-source license is granted for those assets. The archive was initially private; the owner subsequently requested public portfolio access.

Repository-copy validation: the trimmed Git project independently compiled its UE 5.4.4 editor module and cooked all 1,627 LEVEL-6 packages with 0 errors and the same 3 existing warnings. Git LFS integrity checks passed.
