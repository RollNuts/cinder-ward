# Engine Decision

Date: 2026-06-29

## Current Recommendation

Use Godot 4.7 for the first public vertical-slice prototype, while keeping the decision reversible until the first room runs.

## Why Godot First

- MIT license is simple for a commercial Steam game.
- Text-based scenes/resources are friendly to PR review and branch work.
- 2D and 3D can be mixed quickly for a top-down/2.5D test.
- The installed local version is available at `/Users/murakaminaoya/tools/godot/Godot.app`.
- It should be fast enough to prove the first room, lighting, sprite, input, camera, and build path without committing to a heavier production pipeline.

## Why Not Lock Unity Yet

Unity remains strong for 2D tooling, Aseprite integration, Tilemap, Pixel Perfect workflows, and broad Steam production knowledge. The current local Unity install is available, but the project should not default to Unity unless the first-room test proves Godot is weaker for the target.

## Why Not Lock Unreal Yet

Unreal is visually strong for dark 3D spaces, lighting, and post-processing. The current local environment shows Epic/Unreal launcher traces but no confirmed `UnrealEditor.app` binary in the searched locations. Unreal may become relevant if 3D room fidelity is the dominant risk, but it is heavy for the first 2D-centered slice.

## Confirmation Test

Build one running room with:

- Top-down or isometric camera.
- One 96px-readable protagonist.
- One dark room with safe light and outer danger.
- One large threat or pressure source.
- One strike/interact action.
- One local PC build artifact.

If Godot cannot hit the visual target quickly, re-open the engine decision.

