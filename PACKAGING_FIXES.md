# Windows packaging fixes

- Set the default game map to `/Game/LEVEL-6.LEVEL-6`.
- Use a private project PCH and provide a guarded `__has_feature` fallback for the newer local MSVC compiler with UE 5.4.
- Set the two rocket/spaceship child mesh templates to Movable, matching their parent components, to prevent attachment failure in the packaged game.
- Make the gravity manager and spawn-point rifle non-spatially loaded so they are available during player initialization.

The original local project and the full material library are preserved. Changes were implemented and packaged from a separate repair copy. The repository copy omits the original Android File Server security token.

Validation: UE 5.4.4 Windows Development BuildCookRun succeeded; the candidate's runtime log contained zero AttachTo warnings and exited normally. A previous Shipping package also built successfully before the three binary asset fixes. The user reported that the newly opened candidate appeared correct; complete gameplay acceptance remains unverified.

The packaged executable is not stored in this source branch. Launch with `-dx11` on the test machine to avoid the observed DX12 GPU crash.