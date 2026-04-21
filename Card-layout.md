## Card Layout

This document specifies the physical design of cards used in the game.

**Measurement Note:** Use the metric system for all physical component specifications in this project.

---

## Hero Card

Each hero has a **Hero Card** — a durable reference card used during draft, hero selection, and moment-to-moment play. The Hero Card should present the hero's **fixed identity and rules-facing information**, while the Hero Board holds all **changing values** such as current HP, current Mana, gold, cooldowns, and status effects.

The Hero Card is not a substitute for the Hero Board. Its job is to answer: "What kind of hero is this, what are their baseline numbers, and what do their abilities do at each stage of the game?"

### Hero Card Size & Orientation

- **Format:** Oversized portrait card
- **Recommended Size:** 10 × 15 cm
- **Material:** Thick card stock or thin laminated board
- **Back:** Uniform card back for shuffling in All Random and face-down handling during bans or draft piles

This size gives enough room for hero art plus four readable ability blocks without forcing players to handle separate reference sheets during play.

### Information That Belongs On The Hero Card

The Hero Card should show only information that is either static for the whole game or changes in a predictable way by level band.

- Hero name
- Hero portrait / silhouette art
- Class: Strength, Agility, or Intelligence
- Attack type: Melee or Ranged
- Base stats: HP, Mana, Attack, Defense, Move Speed, AP
- Native attack range
- Per-level stat scaling
- Four abilities, including unlock level, activation type, targeting type, AP cost, Mana cost, cooldown, range, duration, and condensed effect text
- Level-band scaling for each ability
- Aghanim's Scepter upgrade text, if applicable
- Role tags for quick teaching and draft readability

### Information That Does Not Belong On The Hero Card

The following should remain on the Hero Board because they change constantly and would create clutter if tracked on the card itself.

- Current HP / Max HP
- Current Mana / Max Mana
- Current level and XP progress
- Gold
- Current AP spent this activation
- Reaction AP debt
- Active cooldown timers
- Active status effects and durations
- Temporary stat bonuses or penalties
- Item slots, item cooldowns, and charges
- Respawn, buyback, and Aegis state

### Relationship To Ability Cards

The Hero Card should include **condensed ability reference text**, not the full exhaustive rules text for every edge case. The separate **Ability Cards** still carry the complete gameplay wording needed during execution and can be slotted onto the Hero Board as they unlock.

This creates a clean three-part system:

- **Hero Card:** identity, baseline stats, progression overview, quick ability reference
- **Ability Cards:** full rules text for each skill
- **Hero Board:** all variable tracking

### Front Face Layout

The Hero Card front should be divided into 5 clear zones.

#### Zone A: Hero Banner

Located at the top 20% of the card.

- Large hero name
- Class icon and color band
	- Strength: red
	- Agility: green
	- Intelligence: blue
- Attack type badge: Melee / Ranged
- 2-3 role tags in small caps
	- Examples: Carry, Support, Nuker, Initiator, Durable, Escape

**Purpose:** Makes the card readable during drafting from across the table.

#### Zone B: Portrait Window

Located just below the hero banner.

- Medium-large hero illustration
- Faint background motif tied to the hero's fantasy
- Optional faction / flavor subtitle

**Purpose:** Preserves Dota identity and makes the roster feel collectible rather than purely utilitarian.

#### Zone C: Base Stat Strip

Located directly under the portrait as a horizontal strip of icons.

**Displayed values:**
- HP
- Mana
- Attack
- Defense
- Move Speed
- AP
- Attack Range

**Presentation:**
- Each stat gets a bold icon and large base number
- Attack Range should be visually tied to attack type
	- Melee: adjacent hex icon
	- Ranged: numeric hex range plus LoS icon

This strip should be readable at a glance without consulting the Hero Board.

#### Zone D: Progression Panel

Located in a narrow band between the stat strip and the abilities.

- **Per Level:** printed once as a compact stat gain line
	- Example: `+10 HP | +10 Mana | +5 ATK | +1 DEF`
- **Unlock Milestones:** small icons for levels 6, 12, and 18
- **Scepter Badge:** star icon with reminder that this hero has a Scepter upgrade

This area exists so players can level correctly without the Hero Card becoming a tracker.

#### Zone E: Ability Grid

This is the main body of the card and should take roughly the bottom half.

Each of the four abilities uses one horizontal row with a consistent mini-template:

- Ability icon
- Ability name
- Unlock level
- Activation type
- Targeting type
- Cost chips: Mana, AP, cooldown
- Range / radius / duration chip when relevant
- One-sentence effect summary
- Mini scaling line

**Recommended scaling shorthand:**
- `1-5:` early-game value
- `6-11:` mid-game value
- `12+:` late-game value
- `18+:` use only when the hero's ultimate has a distinct third breakpoint

This keeps the card aligned with the current hero designs in `Heroes.md`, where most values change by level band rather than every level.

### Ability Row Visual Language

Each ability row should use icons and chips so players can parse it quickly.

- **Type chip:** Passive, Active, Toggle, Channeled
- **Target chip:** Self, Unit, Point, Vector, AoE, Global, Aura
- **Special keyword chip:** Skillshot, Aura, Channel, Scepter
- **Cost chips:** Blue droplet for Mana, gold AP pip for AP, circular arrow for cooldown
- **Range chip:** Hex icon with number
- **Duration chip:** Hourglass icon with turns or rounds label

This matters because `Heroes.md` and `Mechanics.md §17` rely on repeated technical labels. If those labels are standardized visually, players learn the language faster and resolve abilities with fewer rulebook checks.

### Back Face

The Hero Card back should stay uniform for shuffling. If a non-uniform back is ever desired for collector appeal, it should be implemented as a sleeve insert rather than printed directly onto the card so draft modes still work cleanly.

### Example Hero Card Reading Order

The player should be able to scan the card in this order:

1. Identify hero: name, class, attack type, role
2. Confirm baseline stats: HP, Mana, Attack, Defense, Move, AP, attack range
3. Confirm level behavior: per-level scaling and unlock milestones
4. Review ability rows for costs, targeting, and effect summaries
5. Use Ability Cards and Hero Board for detailed resolution and tracking

### Design Notes

- The Hero Card should feel like a **reference dashboard**, not a bookkeeping surface.
- The card must support drafting and teaching, so the top half should be high-clarity and low-text.
- The bottom half can carry denser information because it is mostly read by the owning player.
- Because ranged attacks require LoS and several abilities depend on targeting type, those labels should always be explicit on the card.
- The Hero Board already absorbs all temporary complexity, so the Hero Card can remain attractive and stable instead of token-covered.

### Recommended Hero Card Data Template

Use this structure when turning entries from `Heroes.md` into final print layouts:

| Section | Content |
|---|---|
| Banner | Hero name, class, attack type, role tags |
| Portrait | Hero art, subtitle or visual motif |
| Stat Strip | HP, Mana, Attack, Defense, Move Speed, AP, Attack Range |
| Progression | Per-level stat gains, level 6/12/18 milestones, Scepter badge |
| Ability 1 | Name, unlock, type, target, costs, range, summary, scaling |
| Ability 2 | Name, unlock, type, target, costs, range, summary, scaling |
| Ability 3 | Name, unlock, type, target, costs, range, summary, scaling |
| Ability 4 | Name, unlock, type, target, costs, range, summary, scaling |
