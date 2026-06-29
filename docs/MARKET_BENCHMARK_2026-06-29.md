# Market Benchmark 2026-06-29

This document records what Cinder Ward should learn from current Steam-facing games. It is intentionally focused on what appears on screen and in trailers: silhouette, color, visible pressure, action clarity, and replay hooks. No screenshots, video frames, music, or third-party assets are copied into the repo.

## Official Media Pull

The first visual pass used Steam's official `appdetails` media data, then downloaded representative Steam-hosted screenshots locally for inspection. These files are local research references only and are not committed.

| App | Official media checked | Local observation |
| --- | --- | --- |
| [Dead Cells](https://store.steampowered.com/app/588650/Dead_Cells/) | 13 official screenshots, 1 movie entry. Representative screenshot: [Steam CDN](https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/588650/ss_ac28000ade40cc2fe5c128f32ac98ba33c008a7a.1920x1080.jpg) | The red attack arc, white weapon hit, fire at ground contact, and enemy silhouette sell the frame more than facial detail. |
| [Hades II](https://store.steampowered.com/app/1145350/Hades_II/) | 8 official screenshots, 6 movie entries. Steam listed a `Hades II - v1.0 Launch Trailer` movie entry in the API response. Representative screenshot: [Steam CDN](https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/1145350/ss_ef0f63061d0a0a9a7e46f3b84f125d25330e8f19.1920x1080.jpg) | Small characters remain readable through white body marks, oversized blue attack arcs, and bright red/pink impact centers. |
| [V Rising](https://store.steampowered.com/app/1604030/V_Rising/) | 54 official screenshots, 8 movie entries. Representative screenshot: [Steam CDN](https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/1604030/ss_19d6b903fd65c410af902a8c5f62c820cfe09292.1920x1080.jpg) | Scale comes from environment: black foreground framing, deep paths, and a small readable figure in the middle of heavy scenery. |
| [DREDGE](https://store.steampowered.com/app/1562430/DREDGE/) | 13 official screenshots, 5 movie entries. Representative screenshot: [Steam CDN](https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/1562430/ss_70f88014423ed93eaa111c0d0daca2c500f76908.1920x1080.jpg) | The safe light/distant return point is as important as danger. Cinder Ward needs a warm place to return to inside the dark frame. |

Full Steam API media count pulled for the 10 benchmark apps:

| App | Screenshots | Movie entries |
| --- | ---: | ---: |
| Dead Cells | 13 | 1 |
| Hades II | 8 | 6 |
| V Rising | 54 | 8 |
| DREDGE | 13 | 5 |
| Against the Storm | 10 | 2 |
| Balatro | 12 | 1 |
| Loop Hero | 10 | 2 |
| Unrailed | 6 | 2 |
| Overcooked 2 | 29 | 4 |
| Darkest Dungeon II | 20 | 6 |

## Benchmarks

| ゲーム | Steam / 公式リンク | 画面で売っているもの（暗さ/色/主人公/密度） | 動画・実況で映える瞬間 | 中毒性構造 | Cinder Wardへの示唆 |
|---|---|---|---|---|---|
| Dead Cells | [Steam](https://store.steampowered.com/app/588650/Dead_Cells/) / [official](https://deadcells.com/) | Dark stone spaces plus saturated effects. The protagonist is small, but weapons, motion arcs, and enemies read instantly. | Near-death boss fights, fast recoveries, clean hits, and short retries. | Kill, die, learn, unlock, retry. The run speed stays high. | The first character must feel responsive before the full game exists. Action marks should be larger than the body. |
| Hades II | [Steam](https://store.steampowered.com/app/1145350/Hades_II/) / [official](https://www.supergiantgames.com/games/hades-ii/) | Strong top-down silhouettes, polished character identity, high contrast effects, dense but readable rooms. | Weapon/boon changes, boss phase shifts, and reward selection moments. | Room rewards and build variation make repeated runs feel authored. | Cinder Ward needs room-end choices that visibly change the next room. |
| V Rising | [Steam](https://store.steampowered.com/app/1604030/V_Rising/) / [official](https://www.vrising.com/) | Gothic castles, purple/red magic, moonlit exteriors, and player fantasy that reads from architecture. | Castle expansion, boss hunting, raids, and night/day pressure. | Combat, crafting, and place-making reinforce each other. | The cathedral-city should be a progression object, not only a background. |
| DREDGE | [Steam](https://store.steampowered.com/app/1562430/DREDGE/) / [official](https://www.dredge.game/) | Fog, sea color, tiny player vessel, and readable safety/danger contrast. | Night danger, monster reveals, and limping back to safety with cargo. | Go out, collect, risk more, return, upgrade. | Pressure without a clock works when safety and danger are visible in the world. |
| Against the Storm | [Steam](https://store.steampowered.com/app/1336490/Against_the_Storm/) / [publisher](https://hoodedhorse.com/games/against-the-storm/) | Rain, forest, warm settlement light, and many state indicators without losing the fantasy. | Storm escalation, settlement recovery, and crisis tradeoffs. | Repeated settlements with persistent meta progress. | Use stacked world states, not a visible timer, as the pressure system. |
| Balatro | [Steam](https://store.steampowered.com/app/2379780/Balatro/) / [official](https://www.playbalatro.com/) | Bright readable cards, limited visual vocabulary, high clarity of cause/effect. | Score explosions and combo reveals that viewers understand quickly. | Short rounds, multipliers, and "one more run" escalation. | Even dark fantasy needs clear combinational payoffs. Forge/tool results should pop immediately. |
| Loop Hero | [Steam](https://store.steampowered.com/app/1282730/Loop_Hero/) / [official](https://loophero.com/) | Dark 2D board, symbolic hero, and clear placed tiles. | A built loop turning dangerous, boss meters filling, and retreat decisions. | Placing changes future risk; resources feed camp growth. | "Place" should be a strategic verb with visible future consequences. |
| Unrailed | [Steam](https://store.steampowered.com/app/1016920/Unrailed/) / [official](https://unrailed-game.com/) | Colorful pixel co-op, moving objective, and instantly legible jobs. | Route panic, resource shortages, and last-second fixes. | Clear success/failure for each segment; roles emerge naturally. | Keep carrying/building pressure, but replace the train with district gates and ward engines. |
| Overcooked 2 | [Steam](https://store.steampowered.com/app/728880/Overcooked_2/) / [official](https://www.team17.com/games/overcooked-2/) | High color, low ambiguity, small avatars, dense shared workspace. | Miscommunication, blocked paths, synchronized saves, and chain failures. | Simple verbs combine into chaotic team strategy. | "Sort" must be visible: viewers should know why the team chose the wrong priority. |
| Darkest Dungeon II | [Steam](https://store.steampowered.com/app/1940340/Darkest_Dungeon_II/) / [official](https://www.darkestdungeon.com/darkest-dungeon-ii/) | Heavy gothic silhouettes, candlelight, stress, and travel through hostile space. | Near-collapse recoveries, bad tradeoffs, and grim victories. | Party state, risk, and rewards compound across travel. | Cinder Ward should make damaged states dramatic and readable, not just numeric. |

## Shared Sellable Traits

1. One frame communicates fantasy, objective, and danger.
2. Strong effects are more important than facial detail at gameplay scale.
3. Failure teaches the next attempt instead of feeling like erased time.
4. Viewers can describe what went wrong after a chaotic moment.
5. Progress is visible through tools, room states, route changes, or build choices.

## First Character Requirements

1. Adult, sharp, dangerous silhouette.
2. One readable pale face/mask/helmet mark at small size.
3. One red or gold accent that survives dark rooms.
4. A tool/weapon shape that explains verbs: strike, carry, place, forge.
5. Idle, walk, carry, hit, and interact animations must read before polish.

## Avoid

1. Generic "chosen hero" costume language.
2. Chibi proportions as the first production target.
3. A main countdown timer as the only pressure.
4. A train, wagon, or kitchen surface swap.
5. Beautiful lore that does not produce a clear playable screenshot.
