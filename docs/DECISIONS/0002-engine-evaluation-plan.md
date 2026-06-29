# 0002: Engine Evaluation Plan

Date: 2026-06-29

## Decision

Do not lock the engine before a vertical-slice test. Evaluate Godot, Unity, and Unreal against the same target:

- 2D/2.5D dark fantasy camera.
- One strong protagonist sprite.
- One high-contrast room.
- Real-time lighting or equivalent fake lighting.
- PC build path suitable for Steam.

## Current Bias

Godot is the current practical favorite for a first-week vertical slice because it is lightweight, MIT-licensed, VCS-friendly, and strong enough for 2D/2.5D tests.

Unity remains strong for 2D tooling and Steam-scale production.

Unreal remains strongest for dark 3D look development, but may be heavy for the first 2D-centered vertical slice unless the 3D room quality becomes the dominant risk.

## Confirmation Test

The engine decision must be confirmed with a real running room, not only documentation.

