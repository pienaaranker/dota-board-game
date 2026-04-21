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

---

## Ability Cards

Each hero also has a set of **Ability Cards**. These are the cards players actually use to resolve hero abilities during play. If the Hero Card answers "what does this hero generally do," the Ability Cards answer "how does this specific ability work right now, at the table, without needing the rulebook?"

Ability Cards should contain the **full playable rules text** for a single ability, including targeting, costs, timing, restrictions, scaling, and any special interactions that matter during resolution.

### Relationship To Hero Cards And Hero Boards

The component split should remain strict:

- **Hero Card:** condensed overview of the whole hero
- **Ability Card:** full rules for one specific ability
- **Hero Board:** tracks cooldowns, durations, unlock state, and temporary effects

An Ability Card is a rules reference and play aid, not a tracker. It should not be covered in counters during normal use.

### Ability Card Size & Orientation

- **Format:** Standard portrait card
- **Recommended Size:** 6.3 × 8.8 cm
- **Material:** Standard playing card stock with linen finish
- **Back:** Uniform within that hero's four-card ability set, or fully uniform across all Ability Cards if they may ever be shuffled together during setup or storage

This size keeps ability text readable while still fitting cleanly in the Hero Board's ability area.

### How Many Ability Cards Per Hero

Each hero should have **4 Ability Cards**, one for each named ability.

- 3 basic abilities available from level 1
- 1 ultimate that unlocks at level 6

The same physical Ability Card should usually handle all level-band scaling for that ability rather than creating separate level-up replacement cards, unless later testing shows that the text becomes too dense.

### Information That Belongs On An Ability Card

An Ability Card should contain all information needed to execute the ability correctly in play.

- Hero name
- Ability name
- Ability icon
- Ability slot marker or ordering marker
- Unlock level
- Activation type: Passive, Active, Toggle, Channeled
- Targeting type: Self, Unit, Point, Direction/Vector, AoE, Global, Aura
- Special markers: Skillshot, Aura, Channel, Scepter Upgrade, Toggle
- Mana cost
- AP cost
- Cooldown
- Range
- Radius / line / cone / area shape when relevant
- Duration when relevant
- Full effect text
- Level-band scaling text
- Notes or restrictions required for correct use
- Dedicated Aghanim's Scepter upgrade section if the ability has one

### Information That Does Not Belong On An Ability Card

The following should stay off the card face and be tracked elsewhere.

- Current cooldown marker
- Charges spent this round unless the ability itself uses printed charges as a core mechanic
- Current remaining duration of active effects
- Current mana pool
- Current AP available
- Current level tracker
- Current stacks tracked physically on the Hero Board

### Front Face Layout

The Ability Card front should be divided into 6 functional zones.

#### Zone A: Ability Header

Located at the top of the card.

- Large ability name
- Small hero name above or below it
- Ability icon
- Small slot badge for Ability 1 / 2 / 3 / Ultimate
- Unlock level marker

**Purpose:** Lets players identify the card instantly when multiple hero components are on the table.

#### Zone B: Type And Target Band

Located directly below the header.

- Activation type chip
- Targeting type chip
- Special rule chips where relevant
	- Skillshot
	- Aura
	- Channeled
	- Toggle
	- Global

This band should use standardized icons and vocabulary copied exactly from the rules language in `Mechanics.md §17`.

#### Zone C: Cost And Range Strip

Compact horizontal strip with large icons.

- Mana cost
- AP cost
- Cooldown
- Range
- Duration
- Area icon when relevant

Not every field is required on every card, but the layout should reserve stable positions so players learn where to look.

#### Zone D: Core Effect Text

This is the main rules box.

- Full effect text in plain playable language
- Trigger timing when relevant
- Restrictions and interrupt conditions when relevant

This text should prioritize resolution clarity over flavor. If an ability has a complex edge case that players will encounter regularly, it belongs here rather than being hidden in supporting notes.

#### Zone E: Level Progression Panel

Located below the main rules box.

- Printed scaling by level band
- Use the same shorthand as the Hero Card for consistency:
	- `1-5:`
	- `6-11:`
	- `12+:`
	- `12-17:`
	- `18+:`

This area should be visually distinct from the main effect text so players can scan baseline function separately from level scaling.

#### Zone F: Upgrade / Notes Panel

Located at the bottom of the card.

- Aghanim's Scepter upgrade text, if the ability has one
- Rules notes that are too important to omit but too conditional to sit inside the main effect paragraph

This panel should not be used for flavor text. It exists for gameplay clarity.

### Visual Language

Ability Cards should be more technical and rules-forward than Hero Cards.

- The Hero Card sells identity
- The Ability Card sells clarity

Recommended visual approach:

- Smaller portrait or no portrait at all; use an ability icon instead
- Strong text hierarchy with clean dividers
- Consistent chip system for type, target, costs, and keywords
- A subtle hero-class color accent is acceptable, but the card should primarily be organized by readability rather than faction-color spectacle
- Area-of-effect shapes should use tiny geometric icons when possible: circle, line, cone, self-burst, global

### Readability Rules

Because these are gameplay tools, the card should optimize for fast reading.

- Use short paragraphs rather than dense text walls
- Bold only the most important terms
- Avoid decorative backgrounds behind rules text
- Keep icon usage consistent across all heroes
- If a card includes a Skillshot, mark that explicitly in a highly visible way
- If a card is Channeled or Toggle, those states should be obvious from across the table
- If a card has no Mana cost or no cooldown, print `0` or `None` explicitly instead of leaving the field blank

### Passive, Toggle, And Channeled Cards

These card types need special treatment so they read differently at a glance.

#### Passive Abilities

- Use a muted but clearly labeled Passive chip
- No Mana or AP field is needed unless there is an exception
- Focus the layout on persistent effect text and level scaling

#### Toggle Abilities

- Show `AP to activate` rather than a generic AP cost when relevant
- Show `Cooldown: None` explicitly if it can be toggled freely
- Include a reminder line describing when it can be toggled off

#### Channeled Abilities

- Use a prominent Channeled label
- Include interrupt conditions in the main effect text or a clearly visible notes box
- Include the maximum channel duration if one exists

### Skillshot And Area Marking

Some abilities require more spatial information than others. These should be marked clearly.

- **Skillshot:** visibly labeled so players know the Dodge Skillshot reaction is allowed
- **Line / Vector abilities:** use a line icon and maximum range field
- **AoE abilities:** use a radius or shape icon
- **Global abilities:** use a unique global marker rather than a numerical range
- **Aura abilities:** indicate who is affected and whether the aura is local or global

### Upgrade Philosophy

Ability Cards should assume one-card longevity across the full game.

- A player should not need a new copy of the card at level 12 or 18
- Level scaling should already be printed on the card
- Scepter upgrades should be printed directly on the affected card in a dedicated panel

This matches the current rules in `Mechanics.md`, where Aghanim's Scepter upgrades are explicitly printed on the upgraded ability.

### Recommended Ability Card Data Template

Use this structure when converting hero abilities into final print layouts:

| Section | Content |
|---|---|
| Header | Ability name, hero name, icon, slot, unlock level |
| Type Band | Activation type, targeting type, special tags |
| Cost Strip | Mana, AP, cooldown, range, duration, shape |
| Effect Box | Full rules text, timing, interrupt conditions, restrictions |
| Scaling Panel | Level-band progression |
| Upgrade / Notes | Scepter upgrade and key reminders |

### Design Notes

- Ability Cards should feel like compact rules references, not splashy collectible cards.
- The art can be minimal; icon clarity is more important than illustration space.
- If text density becomes too high for specific heroes, split presentation problems locally rather than weakening the overall system.
- The strongest test of a good Ability Card is whether a player can resolve the ability correctly without opening `Mechanics.md`.
| Ability 4 | Name, unlock, type, target, costs, range, summary, scaling |
