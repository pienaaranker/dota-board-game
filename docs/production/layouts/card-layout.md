## Card Layout

This document specifies the physical design of cards used in the game.

**Measurement Note:** Use the metric system for all physical component specifications in this project.

---

## Hero Card

Each hero has a **Hero Card** — a durable reference card used during draft, hero selection, and moment-to-moment play. The Hero Card should present the hero's **fixed identity and rules-facing information**, while the Hero Board holds all **changing values** such as current HP, current Mana, gold, cooldowns, and status effects.

The Hero Card is not a substitute for the Hero Board. Its job is to answer: "What kind of hero is this, what are their baseline numbers, and what are their four abilities at a glance?" The full rules text and numerical scaling now live on a separate **Abilities Card** for that hero.

### Hero Card Size & Orientation

- **Format:** Oversized portrait card
- **Recommended Size:** 10 × 15 cm
- **Material:** Thick card stock or thin laminated board
- **Back:** Uniform card back for shuffling in All Random and face-down handling during bans or draft piles

This size gives enough room for hero identity, baseline stats, and a compact four-ability overview without forcing variable gameplay tracking onto the card itself.

### Information That Belongs On The Hero Card

The Hero Card should show only information that is either static for the whole game or changes in a predictable way by level band.

- Hero name
- Hero portrait / silhouette art
- Class: Strength, Agility, or Intelligence
- Attack type: Melee or Ranged
- Base stats: HP, Mana, Attack, Defense, Move Speed, AP
- Native attack range
- Per-level stat scaling
- Four abilities, including name, unlock level, activation type, targeting type, and a short effect summary
- A compact reminder that full rules, numbers, and scaling are on the hero's Abilities Card
- Aghanim's Scepter upgrade reminder, if applicable
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

### Relationship To Abilities Cards

The Hero Card should include **condensed ability reference text**, not the full exhaustive rules text and numbers for every edge case. Each hero also comes with one separate **Abilities Card** in landscape orientation that carries the complete gameplay wording, targeting notes, timing restrictions, and numerical scaling for all four abilities.

This creates a clean four-part system:

- **Hero Card:** identity, baseline stats, progression overview, quick ability reference
- **Abilities Card:** full rules text and values for all four hero skills
- **Planning Tokens:** face-down commitment tools for actions and hero abilities
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
- One-sentence effect summary
- Optional tiny reminder icon if the ability has a Scepter upgrade or special keyword

The Hero Card ability grid should remain intentionally compact. It is a recognition and teaching surface, not the place where players parse full numerical ability text during resolution.

### Ability Row Visual Language

Each ability row should use icons and chips so players can parse it quickly.

- **Type chip:** Passive, Active, Toggle, Channeled
- **Target chip:** Self, Unit, Point, Vector, AoE, Global, Aura
- **Special keyword chip:** Skillshot, Aura, Channel, Scepter

This matters because [../../content/heroes/roster.md](../../content/heroes/roster.md) and [../../rulebook/mechanics/Mechanics.md](../../rulebook/mechanics/Mechanics.md) rely on repeated technical labels. If those labels are standardized visually, players learn the language faster and resolve abilities with fewer rulebook checks.

### Back Face

The Hero Card back should stay uniform for shuffling. If a non-uniform back is ever desired for collector appeal, it should be implemented as a sleeve insert rather than printed directly onto the card so draft modes still work cleanly.

### Example Hero Card Reading Order

The player should be able to scan the card in this order:

1. Identify hero: name, class, attack type, role
2. Confirm baseline stats: HP, Mana, Attack, Defense, Move, AP, attack range
3. Confirm level behavior: per-level scaling and unlock milestones
4. Review ability rows for names, targeting, and effect summaries
5. Use the Abilities Card and Hero Board for detailed resolution and tracking

### Design Notes

- The Hero Card should feel like a **reference dashboard**, not a bookkeeping surface.
- The card must support drafting and teaching, so the top half should be high-clarity and low-text.
- The bottom half can carry compact ability summaries, but the dense rules text belongs on the separate Abilities Card.
- Because ranged attacks require LoS and several abilities depend on targeting type, those labels should always be explicit on the card.
- The Hero Board already absorbs all temporary complexity, so the Hero Card can remain attractive and stable instead of token-covered.

### Recommended Hero Card Data Template

Use this structure when turning entries from [../../content/heroes/roster.md](../../content/heroes/roster.md) into final print layouts:

| Section | Content |
|---|---|
| Banner | Hero name, class, attack type, role tags |
| Portrait | Hero art, subtitle or visual motif |
| Stat Strip | HP, Mana, Attack, Defense, Move Speed, AP, Attack Range |
| Progression | Per-level stat gains, level 6/12/18 milestones, Scepter badge |
| Ability 1 | Name, unlock, type, target, short summary |
| Ability 2 | Name, unlock, type, target, short summary |
| Ability 3 | Name, unlock, type, target, short summary |
| Ability 4 | Name, unlock, type, target, short summary |

---

## Abilities Card

Each hero also has one **Abilities Card**. This is a landscape rules reference that presents the complete gameplay wording and numerical values for all four abilities on a single component. If the Hero Card answers "what does this hero do," the Abilities Card answers "how do I execute each of this hero's skills correctly at the table?"

The Abilities Card exists because the Hero Card no longer has enough space to carry full rules text and numeric scaling without becoming crowded. It is a reference aid, not a tracker.

### Relationship To Hero Cards, Planning Tokens, And Hero Boards

The component split should remain strict:

- **Hero Card:** condensed overview of the whole hero
- **Abilities Card:** full rules and values for all four hero abilities
- **Planning Tokens:** face-down commitment tools for actions and hero abilities
- **Hero Board:** tracks cooldowns, durations, unlock state, and temporary effects

The Abilities Card should stay visible during play for reference, but should not be covered in counters during normal use.

### Abilities Card Size & Orientation

- **Format:** Landscape reference card
- **Recommended Size:** 15 × 10 cm
- **Material:** Thick card stock or thin laminated board
- **Back:** Uniform within the hero roster if the card is ever sorted or stored face-down

Landscape orientation is preferred because the component must hold four ability sections with readable rules text and numeric scaling on one card.

### How Many Abilities Cards Per Hero

Each hero should have **1 Abilities Card** covering all four named abilities.

- 3 basic abilities available from level 1
- 1 ultimate that unlocks at level 6

The same physical card should handle all level-band scaling rather than creating replacement components at level 12 or 18.

### Information That Belongs On An Abilities Card

An Abilities Card should contain all information needed to execute the hero's abilities correctly in play.

- Hero name
- Four ability sections with clear slot order
- Ability icons
- Unlock levels
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
- Level-band scaling text with actual numbers
- Notes or restrictions required for correct use
- Dedicated Aghanim's Scepter upgrade section if the hero has one

### Information That Does Not Belong On An Abilities Card

The following should stay off the card face and be tracked elsewhere.

- Current cooldown marker
- Charges spent this round unless the ability itself uses printed charges as a core mechanic
- Current remaining duration of active effects
- Current Mana pool
- Current AP available
- Current level tracker
- Current stacks tracked physically on the Hero Board

### Front Face Layout

The Abilities Card front should be divided into 5 functional zones.

#### Zone A: Hero Header

Located along the left edge or top band of the landscape card.

- Hero name
- Small hero portrait, crest, or silhouette
- Class marker
- Quick legend for icon language used below

**Purpose:** Lets players identify the card instantly when multiple hero components are on the table.

#### Zone B: Ability Summary Strip

Compact strip listing the four abilities in order.

- Ability name
- Slot marker: 1 / 2 / 3 / Ultimate
- Unlock level marker
- Small icon or keyword tag

**Purpose:** Gives players a quick navigation row before they read the full text blocks.

#### Zone C: Four Ability Panels

The main body of the card should use four clearly separated ability panels, arranged in two rows of two or one stacked column depending on readability tests.

Each ability panel should include:

- Ability name and icon
- Activation type and targeting type
- Mana / AP / cooldown / range / duration strip
- Full effect text in playable language
- Level-band scaling with explicit numbers
- Special notes such as Skillshot, Interrupts, or Scepter interaction when relevant

#### Zone D: Upgrade / Notes Band

Located below or beside the main ability panels.

- Aghanim's Scepter upgrade text, if the hero has one
- Shared hero-specific clarifications that affect multiple abilities

#### Zone E: Reference Footer

Small footer used for repeated icon definitions or reminder terms.

- Turns vs rounds legend if needed
- Common icon glossary if the card uses abbreviated symbols

### Visual Language

Abilities Cards should be more technical and rules-forward than Hero Cards.

- The Hero Card sells identity
- The Abilities Card sells clarity

Recommended visual approach:

- Landscape information-first layout
- Strong text hierarchy with clean dividers
- Consistent chip system for type, target, costs, and keywords
- Minimal decorative art; icon clarity and text space matter more than illustration space
- A subtle hero-class color accent is acceptable, but readability should dominate the design

### Readability Rules

Because these are gameplay tools, the card should optimize for fast reading.

- Use short paragraphs rather than dense text walls
- Bold only the most important terms
- Avoid decorative backgrounds behind rules text
- Keep icon usage consistent across all heroes
- If an ability is a Skillshot, mark that explicitly in a highly visible way
- If an ability is Channeled or Toggle, those states should be obvious from across the table
- If an ability has no Mana cost or no cooldown, print `0` or `None` explicitly instead of leaving the field blank

### Upgrade Philosophy

Abilities Cards should assume one-card longevity across the full game.

- A player should not need a new card at level 12 or 18
- Level scaling should already be printed on the card
- Scepter upgrades should be printed directly on the card in a dedicated panel

### Recommended Abilities Card Data Template

Use this structure when converting hero abilities into final print layouts:

| Section | Content |
|---|---|
| Header | Hero name, class marker, portrait or crest |
| Summary Strip | Ability names, slot order, unlock levels |
| Ability 1 Panel | Full rules text, costs, targeting, scaling |
| Ability 2 Panel | Full rules text, costs, targeting, scaling |
| Ability 3 Panel | Full rules text, costs, targeting, scaling |
| Ability 4 Panel | Full rules text, costs, targeting, scaling |
| Upgrade / Notes | Scepter upgrade and shared reminders |

### Design Notes

- Abilities Cards should feel like premium rules references, not collectible mini-cards.
- The strongest test of a good Abilities Card is whether a player can resolve the hero's full kit correctly without opening [../../rulebook/mechanics/Mechanics.md](../../rulebook/mechanics/Mechanics.md).
- If text density becomes too high for a specific hero, rebalance panel proportions before reducing rules clarity.
