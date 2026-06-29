# Game Direction: Cinder Ward

Date: 2026-06-29

## Final Pitch

`Cinder Ward` is a dark fantasy co-op reclamation game for 1-4 players. You are not a chosen hero, a wagon guard, or a train crew. You are a cinder-marked expedition squad breaking into ruined cathedral districts, keeping a portable ward engine alive, and forcing the next gate open while the building collapses, enemies flood in, and resources have to be placed, carried, forged, and routed under pressure.

The sell is simple on screen: a small but dangerous squad in a huge black stone room, warm light cutting through fog, enemies pressing from the dark, and players shouting over whether to carry the cinder core, seal a breach, forge a tool, or abandon a side reward.

## World

The setting is a fallen cathedral-city, not a myth encyclopedia. The city is readable without lore: stone, iron, ash, candles, red carpet, broken altars, rain through open roofs, and a black fog that behaves like a hostile tide.

The old city is not being defended from outside. It is already lost. Each run is an attack into a dead district to recover heat, unlock one more gate, and push the frontier deeper. That keeps the game active and aggressive while preserving the dark fantasy atmosphere.

Visual rules:

- Large black architecture and warm torch/ember light.
- Red, gold, dirty white, and cold blue as small accent colors, not a one-color palette.
- Tall readable character silhouettes, not chibi hero faces.
- Strong action marks: blade arcs, ward flares, thrown cores, door impacts, collapsing beams.
- Every screenshot must show a problem, a player response, and a visible consequence.

## Core Loop

The moment-to-moment loop uses the same broad verbs that make Loop Hero, Unrailed, and Overcooked easy to understand, but the fiction and goals are different.

| Verb | Cinder Ward version | Why it creates tension |
| --- | --- | --- |
| Place | Drop ward stakes, barricade pins, lens mirrors, and temporary bridges into fixed sockets. | The room layout changes under pressure; wrong placement is not instant failure, but it creates worse routes. |
| Carry | Move cinder cores, wounded squadmates, keys, ritual fuel, and heavy tools. | Carrying changes movement and attack options, so the team has to cover the carrier. |
| Make | Forge one-use tools at field anvils: breach nails, flare bombs, chain hooks, lock sigils. | Crafting is fast, physical, and noisy; making the answer can attract the next threat. |
| Sort | Choose which breach, door, enemy pack, reward cache, or wounded ally gets handled first. | The pressure is not a timer. It is a set of bad states that can stack until the room becomes hostile. |

The addictive part is that a room rarely fails because one button was hard. It fails because the squad made a greedy route, placed the bridge too early, carried the wrong object, or left a breach alive for too long. That is readable to viewers and funny when it collapses.

## Clear Conditions

Each stage has a blunt goal:

1. Enter a locked district.
2. Find and move the cinder core.
3. Ignite the main ward engine.
4. Hold the room long enough for the gate mechanism to complete.
5. Escape through the opened gate or dive into an optional side room before leaving.

Long-term goal:

- Reclaim a chain of districts leading to the city heart.
- Each cleared district adds a permanent workshop option, character tool, ward engine module, or route modifier.
- Losing does not reset everything. The district run fails, but unlocked workshop knowledge, rescued specialists, and discovered map branches remain.

Failure conditions:

- Full party down with no recoverable ward charge.
- Ward engine shatters after too many stacked breach states.
- The carried cinder core breaks after repeated drops or enemy strikes.

No fixed countdown timer:

- Danger comes from darkness reclaiming floor space, enemies hearing noise, doors buckling, rooms flooding, bridges cracking, and the ward engine overheating.
- The player sees physical state changes instead of a clock.
- A good team can slow the collapse by playing cleanly; a greedy team can create its own disaster.

## Player Verbs

Base controls should fit on a controller without menu friction:

- Move and dodge.
- Strike or shove.
- Pick up, carry, throw, and drop.
- Place or interact.
- Forge/use current tool.
- Ping/call target for co-op clarity.

The protagonist is directly controlled. A pure support or god-view role is weaker for this project because the user's target is tactile chaos and movement pleasure. The camera can be top-down or 2.5D, but the player should feel the weight of running across stone, grabbing a hot object, sliding it across a bridge, and shoving an enemy back into darkness.

## First Vertical Slice

The first sellable slice is one room, not a full game.

- Character: one adult cinder-marked warden with a long coat or plate silhouette, visible pale face or mask mark, red scarf/sash, short blade, and heavy gauntlet/tool hand.
- Room: a ruined chapel gatehouse with red carpet, broken pillars, two side alcoves, and one central ward engine.
- Enemy: ash thrall pack plus one tall breach knight silhouette.
- Object: one hot cinder core that can be carried, dropped, thrown, damaged, and inserted.
- Tool: one forge station that converts scrap into either a bridge pin or a flare bomb.
- Music states: safe ember, breach pressure, gate ignition, collapse recovery.
- Clear: ignite the ward engine and open the iron gate at the top of the room.

Acceptance test for this slice:

- A screenshot is understandable without text.
- One player can clear it slowly.
- Two players create obvious coordination moments.
- A failed run looks like a sequence of player decisions, not random damage.
- The character still looks dangerous at small size.

## Anti-Goals

- No train, wagon, kitchen, or restaurant surface fiction.
- No chosen-boy hero framing.
- No chibi protagonist as the main sell.
- No belt-action lane progression.
- No main countdown timer.
- No lore names that require a glossary before the action reads.
- No placeholder-looking first character. If the protagonist does not sell the screen, the slice fails.

## Evidence Links

- [Dead Cells on Steam](https://store.steampowered.com/app/588650/Dead_Cells/) for fast readable combat, strong action marks, and replay structure.
- [Hades II on Steam](https://store.steampowered.com/app/1145350/Hades_II/) for top-down combat readability, strong protagonist identity, and room-by-room rewards.
- [V Rising on Steam](https://store.steampowered.com/app/1604030/V_Rising/) for gothic lighting, castle fantasy, and combat/crafting/base progression blend.
- [DREDGE on Steam](https://store.steampowered.com/app/1562430/DREDGE/) for pressure without pure combat, readable night danger, and return-to-safety loops.
- [Against the Storm on Steam](https://store.steampowered.com/app/1336490/Against_the_Storm/) for state pressure and long-form recovery without relying on a simple countdown.
- [Loop Hero on Steam](https://store.steampowered.com/app/1282730/Loop_Hero/) for placing as strategic pressure.
- [Unrailed on Steam](https://store.steampowered.com/app/1016920/Unrailed/) for carrying/building under moving pressure.
- [Overcooked 2 on Steam](https://store.steampowered.com/app/728880/Overcooked_2/) for readable co-op sorting chaos.
