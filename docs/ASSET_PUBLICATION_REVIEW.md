# Asset publication review — 27 October 2026

**Publication decision:** on 27 October 2026, the owner explicitly requested public access for non-commercial portfolio use after this review. That request does not replace the asset licences. The findings and outstanding acquisition-record checks below remain applicable.

## What was checked

- The repository contains vendor-content directories including `ParagonCrunch`, `ParagonGRIMexe`, `AlienBiomassMats`, `Fab`, `Clinic`, `StarterBundle`, `SciFiShelter`, `SciFiDoors` and others.
- The official Paragon: Crunch listing identifies Epic Games as publisher and permits use in Unreal Engine projects. Its public page did not expose a specific acquisition licence in the fetched licence field. A free download or permitted in-game use does not itself establish permission to redistribute the editable source assets publicly.
- The Epic Content License Agreement distinguishes distribution of a built project and rendered images/video from redistribution of source-format licensed content. Section 4 restricts source sharing to the specified development relationships, subject to any applicable service-specific terms.
- The Fab Standard License summary permits sharing assets with collaborators working on a project, including via a private repository, and does not permit standalone asset redistribution. Exact asset listings and the terms applicable when each asset was acquired still need to be matched to the local files.

## Current evidence table

| Local content | Evidence | Public-source status |
| --- | --- | --- |
| `ParagonCrunch` | Official Epic Games listing identified | Not cleared for unrestricted source redistribution |
| `ParagonGRIMexe` | Directory identifies a Paragon asset family; acquisition record not supplied | Not cleared |
| `AlienBiomassMats` | Matching Alien Biomass Materials title found in Fab's material category; exact listing/acquisition terms not established | Not cleared |
| Other Fab/vendor model and material packs | Local directories; no complete per-pack acquisition/licence record located in this review | Not cleared |
| Audio recordings, music, guidance voices | Mixed project audio assets; each asset's creator/source/licence not fully mapped | Not cleared as a complete public source collection |
| Personal Blueprint implementation and documentation | User-confirmed contribution, individual report and implementation screenshots | Suitable material for a scoped portfolio presentation; team ownership and dependencies must remain accurately credited |

## What is still needed for a full-source decision

1. Original store/listing URLs or acquisition records and applicable licences for vendor packs, including the content under `Fab`.
2. Provenance and licence information for sourced audio and music.
3. Any separate written permission permitting public source redistribution where the standard terms do not grant it.

A README credit line or a blanket open-source licence cannot grant rights over third-party assets. Changing only the latest branch would still leave earlier commits and LFS objects within the repository's publication scope. No history rewriting, deletion or repository renaming was performed. The owner subsequently requested a repository visibility change; this does not grant asset-redistribution rights.

If full-source clearance cannot be obtained, a separate public portfolio repository can present the individual's contribution, original documentation, approved implementation material and screenshots, while the complete engineering archive stays private. A packaged demo is a different distribution format and still needs its own asset/attribution checks before release.

## Official sources

- [Epic Content License Agreement, sections 3–4](https://www.unrealengine.com/eula/content)
- [Fab Standard License summary and EULA](https://www.fab.com/eula)
- [Paragon: Crunch — Epic Games](https://www.fab.com/listings/c23ee3a7-4a73-4a83-9061-30b682d269f8)

These findings are an evidence-based publication review, not a claim that every asset uses the same licence or that individual acquisition terms have been verified.
