# DOTA 2: THE BOARD GAME — MOVEMENT AND TERRAIN

This document collects the rules for board structure, action economy, and how heroes move through the map.

---

## The Board

The board represents the battlefield, divided into named areas. Heroes, creeps, and tokens occupy these areas.

### Hex Grid & Terrain
The entire map is built on a **hex grid**. Every hex is one of three terrain types, and some hexes contain structures that further restrict movement:

| Terrain Type | Movement | Line of Sight | Notes |
|---|---|---|---|
| **Open** | Passable | Clear | Default hex — no restrictions. |
| **Tree** | **Blocked** | **Blocked** | Impassable unless an ability says otherwise; blocks LoS; can be destroyed. |
| **Impassable** | **Blocked** | **Blocked** | Permanent walls, cliffs, and water. Cannot be entered or seen through under any circumstances. |

The key difference between **Tree** and **Impassable**: trees can be destroyed and converted to Open hexes; impassable terrain is permanent.

### Buildings & Obstacles
Some hexes contain **structures** that block movement but **do not block Line of Sight**. Heroes can see through them but cannot enter them.

| Structure Type | Movement | Line of Sight | Notes |
|---|---|---|---|
| **Building** | **Blocked** | Clear | Blocks movement; does **not** block LoS. Can be destroyed — once destroyed the hex becomes Open. Examples: base interior walls, reinforcing structures near objectives. |
| **Obstacle** | **Blocked** | Clear | Blocks movement; does **not** block LoS. **Permanent** — cannot be destroyed or removed under any circumstances. Examples: rock formations, fountain pillars, decorative terrain features. |

The key difference between **Building** and **Obstacle**: Buildings can be destroyed through combat (removing the movement block permanently); Obstacles are fixed features of the map.

Neither Buildings nor Obstacles affect LoS — ranged attacks and abilities can target units on the far side of them freely.

Tree clusters contain **Open hexes that wind through them** — these are juke paths. A hero on an Open hex inside a tree cluster is hard to chase because surrounding tree hexes block the enemy's Line of Sight, even though the hero is not inside a tree themselves.

**Named areas** (Jungle Camps, Creep Meeting Points, Roshan's Pit, etc.) are clusters of hexes identified on the board art. When rules reference "being in an area," the hero's token must be on any **Open hex** within that area.

### Tree Destruction
Trees are **mutable terrain** — specific hero abilities and Item Cards can remove them.

- When a tree hex is destroyed it immediately becomes an **Open hex**.
- **All** destroyed trees regrow simultaneously at the end of every **4th Round** (Rounds 4, 8, 12, …), regardless of when they were destroyed during that interval.
- **Tangos** (Item Card): A hero consumes a Tango charge while **adjacent to** a tree hex — that tree is destroyed and the hero restores a fixed amount of Health.
- Other tree-removing effects (e.g., Whirling Death) specify their area of destruction on the hero's Abilities Card.
- An ability that allows a hero to **pass through** tree hexes must explicitly state it on the card.

---

### Lanes
Three lanes run between the two bases: **Top**, **Mid**, and **Bottom**. Each lane has a series of Tower positions and Creep Meeting Points.

### Bases
Each team has a base containing:
- The **Fountain** — restores full Health and Mana to any hero that enters.
- The **Ancient** — the win condition structure.
- **Tier 4 Towers** — two towers guarding the Ancient directly.
- **Barracks** — three buildings inside the base, one corresponding to each lane. Barracks can be sieged once the Tier 3 Tower in their lane has been destroyed.

### River
The central horizontal strip of the map. The **Power Rune** spawns here. Used as a travel and gank corridor.

### Jungle
Unclaimed wilderness areas between lanes on each side of the map. Contains **Neutral Camps** and **Ancient Camps**. Heroes may enter to farm or contest objectives.

### Roshan's Pit
A dedicated area in the river-jungle region. Home to Roshan (see Creeps, Towers, and Objectives).

---

## Action Points (AP) & Actions

Each hero has a fixed AP value printed on their Hero Card. All AP is refreshed at the start of that hero's turn each round.

| Action | AP Cost | Description |
|---|---|---|
| **Move** | 1 | Move the hero token to one adjacent area on the board. |
| **Attack** | 1 | Initiate combat against a specific lane creep token, neutral camp token, Tower, or Enemy Hero in range. There is no separate Farm action. |
| **Deny** | Reaction | Commit a 1 AP reaction during Planning Phase to contest an enemy Attack against an allied lane creep if triggered. Requires a die roll. See Economy and Progression. |
| **Use Item** | Varies | Activate an Item Card's effect by revealing the numbered item slot token for the slot that currently holds that item. Cost listed on the card. |
| **Use Ability** | Varies | Activate a hero ability using the matching hero-specific token. Costs Mana and any AP listed on the hero's Abilities Card. |

---

## Movement

- Each **Move** action costs 1 AP and moves the hero **1 hex** to any of the 6 adjacent hexes.
- Heroes may take multiple Move actions in a turn to travel farther.
- **Tree hexes and Impassable hexes** cannot be entered. Heroes must navigate around them or through Open juke paths within tree clusters.
- Certain hero abilities explicitly allow a hero to blink or pass through tree hexes — this must be stated on the hero's Abilities Card.
- Melee and Ranged heroes move identically; hero type only affects attack range and Line of Sight requirements.
- The **Haste Rune** doubles move efficiency — 1 AP moves the hero **2 hexes** — for its duration.