# DOTA 2: THE BOARD GAME — BOARD LAYOUT & MAP DESIGN

This document defines the physical board layout, named areas, and spatial relationships between game elements. It translates the Dota 2 map into a playable hex-grid board game format.

All entries marked **🔲 TODO** are pending design decisions. Once resolved, the marker is replaced with ✅.

---

## Map Overview ✅ Resolved

**Board Dimensions:** 46 hexes × 46 hexes (2,116 total hexes)

This provides a large playable area with room for:
- Three distinct lanes with proper spacing
- Two full jungle areas (one per team)
- River corridor dividing the map
- Two fortified bases with interior space
- Roshan's Pit
- Adequate tree clusters for juke paths and tactical positioning

**Symmetry:** The map is **largely mirrored diagonally** for Radiant/Dire balance, but **not perfectly symmetrical**. The diagonal runs from bottom-left (Radiant Ancient) to top-right (Dire Ancient). Core strategic elements (lane lengths, tower positions, jungle camp counts, major area sizes) mirror across this axis to ensure competitive fairness. However, **asymmetric features** create the nuance and charm of Dota 2:
- Wall placements and Impassable terrain patterns differ between sides
- Entry points to jungles, bases, and neutral camps vary in position and width
- Tree cluster shapes and juke path geometry are unique per side
- Minor terrain variations create side-specific advantages and disadvantages that balance out over full games

**Orientation:**
- **Radiant (bottom-left corner)** — Player sitting on south/west side of the board
- **Dire (top-right corner)** — Player sitting on north/east side of the board
- Top Lane runs along the top edge, Mid Lane crosses diagonally through center, Bottom Lane runs along the bottom edge

**Visual Design Approach:** Single-piece illustrated board with printed hex grid overlay. Terrain types color-coded (green for Open, dark green/brown for Trees, gray for Impassable). Named areas labeled directly on board art. Tokens used for dynamic elements (heroes, creeps, wards, runes).

---

## Lanes ✅ Resolved

### Lane Structure
Three lanes connect the two bases: **Top**, **Mid**, and **Bottom**.

**Lane paths are defined visually on the board artwork.** Exact distances, widths, and curves are intuitive from the illustrated map. How lanes interact with terrain (tree clusters alongside lanes, choke points, open areas) is determined by the overall terrain distribution design — not specified separately.

### Creep Meeting Points ✅ Resolved
The midpoint between standing towers where creep waves spawn and meet.

**Visual Markers:** Each lane has **multiple pre-defined meeting point hexes** printed directly on the board. These hexes are clearly marked with visual indicators (icons, special coloring, or labeled zones).

**Shifting Rule:** When a tower is destroyed, the meeting point for that lane shifts forward (toward the enemy base) to the next pre-marked hex. **The shift takes effect during the Round End Phase** when new creep waves spawn. This ensures creeps spawn at the new, advanced position after a tower falls, creating lane pressure. Since towers can only be attacked after the lane's creep wave is exhausted (siege requirement), the meeting point naturally updates between waves.

---

## Towers 🔲 TODO

### Tower Positions
Each lane has a sequence of towers: **Tier 1 → Tier 2 → Tier 3**.

**Pending decisions:**
- Exact hex positions for each tower in each lane
- Spacing between tower tiers (how many hexes apart?)
- Tower "zone of control" radius (for siege requirement and Smoke dispel)
- Line of sight from towers (do towers provide vision advantage like Observer Wards?)
- Whether towers are single-hex tokens or multi-hex structures

### Tier 4 Towers
Two towers inside each base, guarding the Ancient.

**Pending decisions:**
- Placement relative to Ancient (flanking positions, distance in hexes)
- Coverage radius
- Whether both must be destroyed or only one to access Ancient

---

## Bases 🔲 TODO

Each team has a fortified base containing the Fountain, Ancient, Barracks, and Tier 4 Towers.

**Pending decisions:**
- Total base size in hexes
- Entry points (how many hexes wide are the openings from each lane?)
- Fountain position and radius (healing area size)
- Ancient position (center of base, or offset?)
- Interior layout (open space vs. maze-like with tree clusters)
- Impassable terrain forming base walls

### Barracks Placement
One Barracks per lane, located inside the base behind the Tier 3 Tower.

**Pending decisions:**
- Exact hex position relative to Tier 3 Tower
- Whether Barracks are single-hex or multi-hex structures
- Separation distance between Top/Mid/Bot Barracks buildings
- Visual distinction on board (icons, tokens, or printed)

---

## River 🔲 TODO

The central horizontal strip dividing the map.

**Pending decisions:**
- River width in hexes
- River terrain type (Open hexes, or special "Water" terrain with movement rules?)
- Whether river provides any mechanical effects (movement speed, vision, etc.)
- Exact path (straight horizontal, or curved/diagonal?)

### Rune Spawn Points
Power Runes spawn at designated river locations.

**Pending decisions:**
- How many rune spawn points? (Dota 2 has two; simplify to one for board game?)
- Exact hex coordinates for spawn point(s)
- Whether rune locations alternate or use fixed position
- Visual marker (printed icon, or token placement zone)

---

## Jungle 🔲 TODO

Wilderness areas on each side of the map, between lanes.

**Pending decisions:**
- Total jungle area size per team (how many hexes?)
- Jungle terrain distribution (ratio of Open hexes to Tree hexes to Impassable)
- Entrances/exits connecting jungle to lanes
- Symmetry enforcement (must both jungles mirror each other exactly?)

### Neutral Camps
Camps containing neutral creeps that can be farmed.

**Pending decisions:**
- Total number of camps per team's jungle
- Camp difficulty distribution (how many Easy / Medium / Hard camps per side?)
- Exact hex positions for each camp
- Camp radius (how many hexes define "being in the camp area"?)
- Respawn marker visibility (printed on board, or separate token?)

### Ancient Camps
High-value neutral camps located deeper in the jungle.

**Pending decisions:**
- How many Ancient camps per team? (Dota 2 has 2 per side; simplify to 1?)
- Exact hex positions
- Proximity to lanes vs. deep jungle placement (risk/reward balance)
- Visual distinction from regular neutral camps

---

## Roshan's Pit 🔲 TODO

Dedicated area in the river-jungle border region.

**Pending decisions:**
- Exact hex position (closer to Radiant or Dire, or centered?)
- Pit size in hexes
- Entry points (how many hexes wide? single choke point or multiple entrances?)
- Interior layout (open area or tree clusters for juking?)
- Whether the pit is elevated/depressed terrain (visual only, or mechanical impact?)
- Aegis drop location (center of pit, or specific hex?)

---

## Secret Shops 🔲 TODO

Hidden shops located in the jungle, allowing item purchases without returning to Fountain.

**Pending decisions:**
- Include Secret Shops at all, or exclude for simplicity? (candidates for exclusion)
- If included: how many per side? (Dota 2 has 1 per team)
- Exact hex positions
- Proximity to lanes vs. deep jungle (risk entering enemy territory to shop)
- Purchasing rules (instant like Fountain, or requires Courier delivery?)
- Limited item pool vs. full shop access

---

## Outposts 🔲 TODO

Capture points located in the jungle that grant XP and provide a forward teleport destination.

**Pending decisions:**
- Include Outposts at all, or exclude for simplicity? (candidates for exclusion; teleport mechanics not yet defined)
- If included: how many per side? (Dota 2 has 2 total, 1 per jungle)
- Exact hex positions
- Capture mechanics (AP cost, can enemies contest?)
- XP reward structure (per-round passive, or one-time capture bonus?)
- Whether Outposts replace Secret Shops or coexist

---

## Terrain Distribution 🔲 TODO

Hex-by-hex allocation of terrain types across the map.

**Pending decisions:**
- Overall ratio of Open : Tree : Impassable hexes
- Tree cluster patterns (large continuous forests vs. scattered groves?)
- Juke path design (how many Open hexes wind through tree clusters? how wide?)
- Impassable terrain distribution (bases, cliffs, river boundaries, decorative features)
- Symmetry enforcement (must terrain mirror perfectly for balance?)

### Juke Paths
Open hexes winding through tree clusters, used for escapes and vision-blocking maneuvers.

**Pending decisions:**
- Named juke path locations (e.g., "Top Lane Treeline," "River Juke")
- Path width (1 hex, or 2+ hexes wide?)
- Path length and complexity (simple shortcuts vs. labyrinthine)
- Whether juke paths connect multiple areas (lane to jungle, jungle to river, etc.)

---

## Ward Spots 🔲 TODO

Optimal hexes for placing Observer Wards and Sentry Wards.

**Pending decisions:**
- Designate "premium" ward spots on the board (printed markers, or player discovery?)
- Coverage overlap analysis (which ward spots cover multiple key areas?)
- Offensive vs. defensive ward zones (deep enemy territory vs. your own jungle)
- Counter-warding hotspots (common Sentry Ward placement to deward enemy Observers)
- Whether ward spot designation is a teaching tool or affects mechanics

---

## Elevation & High Ground 🔲 TODO

Dota 2 features high ground / low ground elevation that affects vision and combat. **High ground advantage was excluded in Mechanics.md**, but elevation may still exist for thematic/visual purposes.

**Pending decisions:**
- Include elevation as visual-only (no mechanical impact), or exclude entirely?
- If visual-only: mark high ground hexes with color/shading for thematic flavor
- River banks as low-to-high transitions
- Base interiors as elevated platforms
- Roshan pit as depressed terrain

---

## Distances & Measurements 🔲 TODO

Key distance relationships that affect gameplay pacing.

**Pending decisions:**
- Fountain to Tier 1 Tower (how many hexes/Move actions to reach lane from spawn?)
- Tier 1 to Tier 2 Tower spacing
- Tier 2 to Tier 3 Tower spacing
- Lane to nearest Jungle Camp (farming rotation efficiency)
- Jungle Camp to Jungle Camp (neutral farming paths)
- Rune spawn to lane (contest timing)
- Roshan Pit to nearest lane (gank escape routes)
- Ancient to Ancient (total map traversal for global abilities and respawn-to-frontline timing)

---

## Visual Design 🔲 TODO

How the board is physically produced and presented.

**Pending decisions:**
- Illustrated single-piece board vs. modular hex tiles
- Art style (top-down Dota 2 map aesthetic, or stylized/abstract?)
- Hex size (large enough for tokens + readable terrain icons)
- Color coding (Radiant side green/gold, Dire side red/purple?)
- Iconography for terrain types (tree symbol, impassable ×, open blank)
- Whether named areas are printed on board or referenced in rulebook only

---

## Design Priorities 🔲 TODO

Strategic goals for the board layout.

**Pending decisions:**
- Emphasize lane dominance (shorter lanes, closer towers) or jungle control (larger jungle with more camps)?
- Roshan contest frequency (central location for constant fights, or offset to create strategic windows?)
- Juke/escape potential (many tree clusters for tactical plays, or open terrain for brawling?)
- Symmetry strictness (perfect mirror for competitive fairness, or asymmetric features for variety?)

---

## Excluded Map Features

The following Dota 2 map elements are **not included** in the board game, either for simplicity or because their parent mechanics were excluded.

| Map Feature | Reason for Exclusion |
|---|---|
| **Bounty Rune Spawn Points** | Bounty Runes excluded in Mechanics.md (redundant with Passive Income). |
| **Tormentor Locations** | Tormentor excluded in Mechanics.md (Aghanim's Shard removed). |
| **Lotus Pool** | Tormentor reward; parent mechanic excluded. |
| **Scan Mechanic** | Not a physical location; global ability not suited to board game. |
| **Shrines** | Removed from Dota 2 in recent patches; outdated mechanic. |
| **Side Shops** | Removed from Dota 2 in recent patches; Secret Shops cover forward purchasing. |
