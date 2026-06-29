# Audio Direction: Cinder Ward

Date: 2026-06-29

## Goal

The audio must make the game feel physical before it feels orchestral. Cinder Ward should not sound like generic heroic fantasy. It should sound like boots on wet stone, a hot core burning through gloves, iron doors bending, a ward engine coughing back to life, and a squad making bad decisions in a huge dark room.

The mix target is dark, readable, and dry enough for action clarity. Music supports the room state; sound effects sell the verbs.

## Benchmarks

| Game | What to study | Cinder Ward takeaway |
| --- | --- | --- |
| [Dead Cells](https://store.steampowered.com/app/588650/Dead_Cells/) | Fast combat transients, attacks that cut through busy music, clear hit confirmation. | Strike, shove, throw, and enemy hit sounds must be short, sharp, and readable even in chaos. |
| [Hades II](https://store.steampowered.com/app/1145350/Hades_II/) | Room-by-room intensity shifts and strong ability identity. | Each tool needs a distinct sonic signature; music should make reward rooms feel like relief. |
| [V Rising](https://store.steampowered.com/app/1604030/V_Rising/) | Gothic ritual weight, castle ambience, dark magic without losing readability. | Ward engines, iron gates, and forge stations should sound heavy and expensive. |
| [DREDGE](https://store.steampowered.com/app/1562430/DREDGE/) | Threat that grows through ambience, night sounds, and return-to-safety contrast. | Danger can rise through room tone and enemy proximity, not through a clock beep. |
| [Darkest Dungeon II](https://store.steampowered.com/app/1940340/Darkest_Dungeon_II/) | Stress, carriage travel, grim impacts, and oppressive musical restraint. | Failure states should sound like pressure stacking, not arcade failure jingles. |
| [Loop Hero](https://store.steampowered.com/app/1282730/Loop_Hero/) | Repetition that becomes hypnotic rather than annoying. | Long sessions need loops with layers that enter/exit based on state. |
| [Unrailed](https://store.steampowered.com/app/1016920/Unrailed/) / [Overcooked 2](https://store.steampowered.com/app/728880/Overcooked_2/) | Readable co-op interaction sounds and quick success/failure feedback. | Carry/place/make/sort actions need immediate sounds that viewers understand without UI text. |

## Music States

Music is state-based, not timer-based.

| State | Use | Sound |
| --- | --- | --- |
| Safe ember | Initial room entry, no breach active. | Low stone air, ember hiss, distant bell, sparse low drone. |
| Search | Players split to find tools/core. | Slow pulse, plucked motif, low bowed texture, lots of space for footsteps. |
| Breach pressure | Enemy entry or darkness reclaiming floor. | Added percussion, distorted breath/noise layer, higher string scrape. |
| Gate ignition | Core inserted, room objective close to success. | Rhythmic lift, bell harmonics, brighter metallic overtones. |
| Collapse recovery | After near failure, revive, or final escape. | Music thins; impacts and room destruction take priority. |

No global countdown sting. If urgency rises, it must be because the room sounds worse: more enemies, buckling doors, unstable ward engine, or core overheating.

## Sound Effect Priorities

The first playable slice needs these before a full soundtrack:

1. Footsteps on stone, carpet, metal grate, and ash.
2. Pick up, carry strain, drop, throw, and core impact.
3. Place ward stake, socket lock, failed placement.
4. Forge station start, loop, completion, and tool pickup.
5. Sword/gauntlet strike, shove, enemy hit, enemy death.
6. Breach open, darkness advance, door buckle, pillar crack.
7. Ward engine idle, charge, overload, shatter, and ignition.
8. Ping/call sound for co-op target sharing.
9. Downed player, revive start, revive complete.
10. Stage clear gate opening.

Each important action needs a short "front" transient and a quieter tail. The front tells the player what happened; the tail sells material and space.

## Free / Commercial-Safe Source Policy

Use original recordings and CC0 first. If an asset requires attribution, it must go into the asset ledger before use.

| Source | Use | Commercial note |
| --- | --- | --- |
| [Kenney](https://kenney.nl/) | UI blips, simple game SFX, placeholder audio. | Kenney assets are commonly provided under permissive terms, but record the exact asset page/license at download time. |
| [Freesound](https://freesound.org/help/faq/) | Foley, impacts, ambience. | Licenses vary by file. Use CC0 where possible; CC BY only with attribution ledger; avoid NonCommercial. |
| [OpenGameArt](https://opengameart.org/) | Temporary music/SFX exploration. | License varies per asset. Use only CC0/CC BY-compatible assets for commercial work. |
| [Sonniss GDC Game Audio Bundles](https://sonniss.com/gameaudiogdc) | Broad SFX library for commercial-safe production candidates. | Keep bundle license/readme with the project and record each selected file. |
| Self-recorded audio | Best source for boots, cloth, metal, stone, breath, tool handling. | Safest if recorded by the team and stored with source notes. |

Do not use ripped game audio, trailer audio, OST stems, YouTube downloads, or samples with unclear redistribution rights.

## Tooling

- Audacity for cleanup, trimming, normalization, and quick batch exports.
- GarageBand, LMMS, or Reaper trial/owned license for cue sketches.
- Surge XT or Vital Free for drones, pulses, and distorted breath layers.
- Godot, Unity, or Unreal implementation should use the same event names and state machine so the engine decision does not invalidate the audio plan.

Suggested event names:

- `player.step.stone`
- `core.pickup`
- `core.drop.heavy`
- `ward.place.ok`
- `ward.place.fail`
- `forge.loop`
- `breach.open`
- `gate.ignite`
- `team.ping`

## First Slice Audio Acceptance

The first room passes audio direction only if:

- A viewer can tell when an object is picked up, dropped, placed, forged, or inserted without reading UI.
- The safe area and dark area sound different.
- The ward engine state is audible before it is visible.
- Combat hits are clear under music.
- The mix leaves room for voice chat and streamer commentary.
