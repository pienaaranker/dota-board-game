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

## Towers ✅ Resolved

### Tower Positions
Each lane has a sequence of towers: **Tier 1 → Tier 2 → Tier 3**.

Tower positions, spacing, health, range, and zone of control are defined on the visual map design and in the dedicated Towers rules document. On the board, each tower occupies a single printed hex with a clear tower icon indicating its tier and team.

### Tier 4 Towers
Two towers inside each base, guarding the Ancient. Both must be destroyed before the Ancient can be attacked. Positions are defined on the board artwork.

---

## Bases 🔲 TODO

Each team has a fortified base containing the Fountain, Ancient, Barracks, and Tier 4 Towers. Exact positions of all structures are defined on the visual board artwork.

**Pending decisions:**
- Entry points: how many lane openings lead into the base, and are they wide enough for multiple heroes to enter simultaneously or are they choke points?
- Interior layout: open space (large area heroes can freely maneuver) or deliberate structure placement limiting movement paths?

### Barracks
One Barracks per lane, printed on the board. Each Barracks is a single-hex structure with a clear icon linking it to its lane.

---

## River 🔲 TODO

The central strip dividing the map between Radiant and Dire territory. Path and shape are defined on the visual board artwork.

**Pending decisions:**
- Terrain type: are river hexes plain **Open** hexes (no special rules), or does the river have a distinct terrain type with movement implications?
- Mechanical effects: does moving through the river have any effect (e.g., slower movement), or is it purely cosmetic?

### Rune Spawn Points
Power Runes spawn at designated river locations. Spawn point(s) are printed on the board.

**Pending decision:**
- How many rune spawn points? Dota 2 has two (one each side of the river). Simplify to **one central point**, or keep two to create a contest over which side claims it?

---

## Jungle 🔲 TODO

Wilderness areas on each side of the map, between lanes. Terrain distribution and entry points are defined on the visual board artwork; the asymmetry between Radiant and Dire jungles is intentional.

**Pending decisions:**
- Terrain feel: should the jungle be dense (mostly Trees with narrow Open paths, high juke potential) or open (more Open hexes with scattered tree clusters, easier to navigate)?
- Entrances: how many distinct entry/exit paths connect the jungle to each adjacent lane?

### Neutral Camps
Camps containing neutral creeps, printed on the board. A hero is "in a camp" when on any hex within the camp's marked area.

**Pending decisions:**
- How many neutral camps per team's jungle?
- Difficulty distribution: how many Easy, Medium, and Hard camps per side?

### Ancient Camps
High-value neutral camps located deep in the jungle, printed on the board with a distinct icon.

**Pending decision:**
- How many Ancient camps per team? Dota 2 has 2 per side — keep both, or simplify to 1 for a cleaner jungle layout?

---

## Roshan's Pit 🔲 TODO

Dedicated area in the river-jungle border region. Exact position and size are defined on the visual board artwork.

**Pending decisions:**
- Positioning: closer to Radiant, closer to Dire, or perfectly centered? (Dota 2 traditionally favors Radiant-side, creating a minor strategic asymmetry.)
- Entry points: single choke point entrance (high-stakes, easy to contest) or multiple entrances (more dynamic fights, harder to defend)?
- Interior layout: open pit (straightforward fight) or tree clusters inside (juking possible, adds chaos to Roshan fights)?

---

## Secret Shops 🔲 TODO

Hidden shops located in the jungle allowing forward item purchases without returning to the Fountain. One per team in Dota 2.

**Pending decisions:**
- Include or exclude? Forward purchasing adds strategic depth (jungling heroes can buy without recalling) but adds board complexity.
- If included: placement in own jungle only, or accessible from enemy territory too (high-risk reward)?
- If included: same full item pool as Fountain, or limited to a subset of items? (Purchasing rules would be defined in the Items document.)

---

## Outposts 🔲 TODO

Capture points in the jungle that grant XP and act as forward teleport destinations. One per side in Dota 2.

**Pending decisions:**
- Include or exclude? Teleport mechanics are not yet defined — if teleportation doesn't exist in this game, Outposts lose their main purpose and should be excluded.
- If teleportation is added: do Outposts coexist with Secret Shops, or replace them as the key mid-jungle objective?

---

## Terrain Distribution 🔲 TODO

The overall character of the map determined by how Open, Tree, and Impassable hexes are distributed. Exact hex-by-hex placement is defined on the visual board artwork.

**Pending decisions:**
- Map feel: dense and tactical (heavy tree coverage, many choke points) or open and aggressive (wide lanes, sparse jungle)?
- Tree cluster style: large continuous forests with winding paths, or scattered smaller groves throughout?
- Impassable terrain use: primarily for base walls and river banks, or also used to create cliff features and broken terrain across the map?

### Juke Paths
Open hexes winding through tree clusters. Named juke paths and their locations are labeled on the visual board artwork.

**Pending decision:**
- Path width: single-hex paths (narrow, harder to chase through) or 2-hex wide paths (more forgiving, easier to navigate)?

---

## Ward Spots 🔲 TODO

Optimal hexes for placing Observer and Sentry Wards. Specific high-value positions emerge naturally from the board layout.

**Pending decision:**
- Should premium ward spots be **printed on the board** as visual guides (teaching tool for new players, no mechanical effect), or left entirely to player discovery?

---

## Elevation & High Ground 🔲 TODO

High ground advantage was excluded in Mechanics.md. However, elevation can still exist as a visual layer on the board.

**Pending decision:**
- Visual elevation only (bases shaded as elevated, river as low ground, Roshan's Pit as depressed — no mechanical effect), or exclude elevation entirely from the artwork to keep the board cleaner?

---

## Distances & Measurements

All key distances (Fountain to lane, tower spacing, jungle camp proximity, rune timing) are determined by the visual board design. No separate specification needed — distances emerge from structure placement on the 46×46 grid and are validated during playtesting.

---

## Visual Design

Already established in Map Overview: single-piece illustrated board with printed hex grid overlay. Terrain color-coded, named areas labeled on board art, tokens for dynamic elements.

Art direction decisions (style, color palette, iconography, hex size) are outside the scope of this rules/layout document and belong to the production design phase.

---

## Design Priorities 🔲 TODO

Strategic goals that guide all remaining layout decisions.

**Pending decisions:**
- Balance emphasis: lane dominance (tighter lanes, towers closer together) or jungle control (larger jungle with more camps to contest)?
- Roshan: centrally located for frequent early contests, or offset to create deliberate strategic windows?
- Tactical texture: many tree clusters and choke points for high juke/escape potential, or more open terrain favoring direct brawling?

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
