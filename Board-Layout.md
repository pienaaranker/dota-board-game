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

## Bases ✅ Resolved

Each team has a fortified base containing the Fountain, Ancient, Barracks, and Tier 4 Towers. Exact positions of all structures are defined on the visual board artwork.

**Entry Points:** Three openings — one per lane — each **3 hexes wide**. Wide enough for multiple heroes to push or defend simultaneously without creating a single-file choke point.

**Interior Layout:** The base interior is not open space — **Buildings and Obstacles** are placed throughout to create deliberate movement paths, protect key structures, and reward positional play. Heroes cannot freely maneuver to any hex; they must navigate around these structures to reach the Barracks, Tier 4 Towers, and Ancient.

### Barracks
One Barracks per lane, printed on the board. Each Barracks is a single-hex structure with a clear icon linking it to its lane.

---

## River ✅ Resolved

The central strip dividing the map between Radiant and Dire territory. Path and shape are defined on the visual board artwork.

River hexes are plain **Open** hexes — no movement penalties or special rules. The river is a cosmetic feature that visually separates the two halves of the map and provides a travel corridor.

### Rune Spawn Points ✅ Resolved
Two rune spawn points are printed on the board — one on the Radiant side of the river, one on the Dire side.

At the **start of every 4th round**, any player simultaneously rolls the **custom Rune Die** (determines rune type) and flips a **coin** (determines which side spawns it). Both results are resolved together. Only one rune is on the board at a time.

---

## Jungle ✅ Resolved

Wilderness areas on each side of the map, between lanes. Terrain distribution and entry points are defined on the visual board artwork; the asymmetry between Radiant and Dire jungles is intentional.

### Neutral Camps ✅ Resolved
Camps containing neutral creeps, printed on the board. A hero is "in a camp" when on any hex within the camp's marked area.

Each team's jungle is divided into two sections by lane proximity:

**Safe Lane Jungle** — 3 camps, one of each difficulty:
- 1 Easy Camp
- 1 Medium Camp
- 1 Hard Camp

**Off Lane Jungle** — 2 camps:
- 1 Medium Camp
- 1 Ancient Camp

### Ancient Camps ✅ Resolved
One Ancient Camp per team, located in the off lane jungle. Printed on the board with a distinct icon to distinguish it from regular neutral camps.

---

## Roshan's Pit ✅ Resolved

Dedicated area in the river-jungle border region, positioned on the **Dire side** between the Dire mid lane and off lane — mirroring the traditional Dota 2 placement. Exact position and size are defined on the visual board artwork.

**Positioning:** Nudged into Dire territory, creating a minor asymmetry — slightly easier for Dire to defend and slightly riskier for Radiant to contest.

**Entry Point:** Single entrance, mouth **facing the Radiant side**. One way in, one way out — creating a high-stakes choke point for both attacking and defending teams.

**Interior:** Small, fully open space. No trees, buildings, or obstacles inside. The pit is compact enough that the fight plays out in the open with no positional complexity inside — the strategic tension comes entirely from controlling the entrance.

---

## Secret Shops ✅ Resolved

One Secret Shop per side, printed on the board. Positioned near the **off lane Ancient Camp** in each team's jungle.

**Access:** Any hero — from either team — may purchase from either Secret Shop by moving into its area. Entering enemy jungle to shop carries inherent risk.

**Item Pool:** A limited subset of items is available at Secret Shops; not the full Fountain catalogue. The exact item list is defined in the Items document.

---

## Terrain Distribution ✅ Resolved

The overall character of the map determined by how Open, Tree, and Impassable hexes are distributed. Exact hex-by-hex placement is defined on the visual board artwork.

**Buildings** appear exclusively inside the two bases, creating deliberate interior movement paths around key structures (Barracks, Tier 4 Towers, Ancient). Destroyable — once cleared, the path becomes open.

**Obstacles** are scattered across the map, concentrated in jungle areas. They serve as permanent decorative and structural features (rock formations, ruins, pillars) that create non-linear movement paths, interesting positional decisions, and visual character without blocking sight lines.

### Juke Paths
Open hexes winding through tree clusters, created organically by tree positioning on the board. Juke paths are not labeled or named — players discover and exploit them through play.

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
| **Outposts** | Teleport mechanics not included in this game; without teleportation, Outposts serve no purpose. |}
