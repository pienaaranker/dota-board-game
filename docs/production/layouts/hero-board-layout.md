# DOTA 2: THE BOARD GAME — HERO BOARD LAYOUT & TRACKING SYSTEM

This document specifies how all game variables are tracked using physical, offline components: cardboard mats, tokens, dice, sliders, and cards. No companion apps, no digital tracking — everything is tactile and visible.

**Measurement Note:** Use the metric system for all physical component specifications in this project.

---

## Individual Hero Board (Player Mat)

Each player receives a **Hero Board** — a large printed cardboard mat (approximately 30 × 40 cm) that holds the hero's generic planning and tracking surfaces. Variable numeric values such as HP, Mana, AP, Level, XP, Gold, and similar counters are handled by a separate **3D-printed stat tracker**, not printed directly on the Hero Board. The board is divided into functional zones.

### Zone 1: Base Stats Reference

Located at the top of the mat. The Hero Board shows only the hero's static printed reference stats. Live numeric values are handled on the separate **3D-printed stat tracker**.

#### Static Stats Display
- **Component:** Printed boxes with **stackable +1 tokens** for modifications
- **Stats displayed:**
  - **Attack** — Base value printed. Add red +1/+5/+10 tokens for item/buff bonuses.
  - **Defense** — Base value printed. Add gray +1/+5 tokens for item/buff bonuses.
  - **Move Speed** — Base value printed. Add green +1 tokens for item/buff bonuses.
  - **AP per Turn** — Base value printed. Stun penalties tracked separately (see Status Effects).

---

### Zone 2: Action Planning & Duration Tracking

Located in the center of the mat. This zone serves two purposes: staging face-down planning tokens for the current turn and tracking all time-based effects.

#### Planning Token Staging Area
Located at the top of Zone 2.

- **Component:** Rectangular zone labeled "Action Queue"
- **Size:** Fits up to 10 planning tokens laid horizontally in sequence
- **Usage:** During Planning Phase, place selected tokens face-down here in the order you want to execute them. During your activation, reveal and execute from left to right.

#### Printed Quick Reference Panel
- **Component:** A compact printed rules-reference panel placed in the open space between the action-planning area and the item / backpack area
- **Usage:** Provides high-frequency reminders so players do not need a separate helper card for core turn flow and item handling
- **Printed Copy:**
  - **PLAN** — Commit actions and reactions
  - **REVEAL** — Resolve **left to right**; choose targets on reveal
  - **MOVE** — Move **1 hex**
  - **ATTACK** — Damage enemies and kill creeps
  - **ABILITY | ITEM** — Use hero skills and active items
  - **REACTIONS** — Respond to enemy actions
  - **COMBAT** — Apply damage after defense
  - **ROUND END** — Resolve round upkeep

---

#### Dual Duration Tracking System

Located below the planning area. Divided into two parallel sections for different time measurements.

**Left Section: TURNS (10 compartments)** | **Right Section: ROUNDS (6 compartments)**

Each section contains two rows of tracking compartments:

**Design Constraint:** Maximum cooldown for any ability or item is **5 rounds**. Round values are tracked as: ½, 1, 2, 3, 4, 5.

---

##### Turn-Based Tracking (Left Section)

**Status Durations Row (Top)**
- **Component:** Horizontal strip with **10 vertical compartments**
- **Marker:** Place status effect tokens (Stunned, Silenced, Rooted, etc.) in compartments with small numbered token showing turns remaining
- **Usage:** For effects that expire after X turns (individual hero activations). Move token forward or decrement counter each time this hero activates.
- **Maximum Duration:** Up to 10 turns can be tracked simultaneously

**Ability Cooldowns Row (Bottom)**
- **Component:** Horizontal strip with **10 vertical compartments**
- **Marker:** Place small ability identifier tokens with numbered token showing turns remaining
- **Usage:** For abilities with cooldowns measured in turns. Decrement each time this hero activates.
- **Maximum Duration:** Up to 10 turns can be tracked simultaneously

---

##### Round-Based Tracking (Right Section)

**Status Durations Row (Top)**
- **Component:** Horizontal strip with **6 vertical compartments**
- **Values Tracked:** ½ round, 1, 2, 3, 4, 5 rounds
- **Marker:** Place status effect tokens (BKB Active, Ethereal, etc.) in compartments with small numbered token showing rounds remaining
- **Usage:** For effects that expire after X rounds (all 20 hero activations). Decrement at Round End Phase.
- **Maximum Duration:** 5 rounds (design constraint)

**Ability Cooldowns Row (Bottom)**
- **Component:** Horizontal strip with **6 vertical compartments**
- **Values Tracked:** ½ round, 1, 2, 3, 4, 5 rounds
- **Marker:** Place small ability identifier tokens (Q, W,─────────┐
│             PLANNING TOKEN STAGING AREA                         │
│    [Token] [Token] [Token] [Token] [Token] ...                 │
└──────────────────────────────────────────────────────────────────┘

┌───────────────────────────────┬──────────────────────────────────┐
│    TURNS (10 compartments)    │   ROUNDS (6 compartments)        │
├───────────────────────────────┼──────────────────────────────────┤
│ Status Durations              │ Status Durations                 │
│ ┌──┬──┬──┬──┬──┬──┬──┬──┬──┬─┐│ ┌──┬──┬──┬──┬──┬──┐             │
│ │  │  │  │  │  │  │  │  │  │ ││ │½ │1 │2 │3 │4 │5 │             │
│ └──┴──┴──┴──┴──┴──┴──┴──┴──┴─┘│ └──┴──┴──┴──┴──┴──┘             │
├───────────────────────────────┼──────────────────────────────────┤
│ Ability Cooldowns             │ Ability Cooldowns                │
│ ┌──┬──┬──┬──┬──┬──┬──┬──┬──┬─┐│ ┌──┬──┬──┬──┬──┬──┐             │
│ │  │  │  │  │  │  │  │  │  │ ││ │½ │1 │2 │3 │4 │5 │             │
│ └──┴──┴──┴──┴──┴──┴──┴──┴──┴─┘│ └──┴──┴──┴──┴──┴──┘             │
└───────────────────────────────┴──────────────────────────────────┘
```

**Section Distribution:**
- **Turns Section:** 10 compartments (2 rows × 10 each) — tracks turn-by-turn effects and cooldowns
- **Rounds Section:** 6 compartments (2 rows × 6 each) — tracks round-based effects: ½, 1, 2, 3, 4, 5 rounds
- **Maximum Cooldown Constraint:** No ability or item cooldown exceeds 5 rounds

**Design Notes:**
- Most ability cooldowns use the **Rounds** section (right side)
- Most status effects use the **Turns** section (left side) for precise control
- Items with turn-based cooldowns (e.g., Phase Boots) use **Turns** section
- Items with round-based cooldowns (e.g., Black King Bar) use **Rounds** section
- The labeled round compartments (½, 1, 2, 3, 4, 5) make tracking explicit and prevent confusion
```

**Design Notes:**
- Most ability cooldowns use the **Rounds** section (right side)
- Most status effects use the **Turns** section (left side) for precise control
- Items with turn-based cooldowns (e.g., Phase Boots) use **Turns** section
- Items with round-based cooldowns (e.g., Black King Bar) use **Rounds** section
- The 6 compartments per row provide ample space for simultaneous effects
- Numbered tokens (D6 dice or small number markers) placed on status/ability tokens show remaining duration
- The same generic tracks can also hold non-ability timers such as a dead hero's respawn position, Buyback cooldown, Aegis expiration, or courier delivery countdown when those states are represented by dedicated tokens

---

### Zone 3: Item Slots And Backpack

Located in the center-right of the mat. This zone contains **6 active item slots** and a separate **3-slot backpack**.

#### Active Item Slots (×6)
- **Component:** Standard card slot (fits Item Cards)
- **Printed Identity:** Each slot is clearly labeled **1** through **6** to match the hero's numbered item planning tokens
- **Card displays:** Item name, stats/bonuses, active effect (if any)

#### Backpack Slots (×3)
- **Component:** Standard card slots grouped beside the active item area under a clear **Backpack** label
- **Usage:** Backpack items are carried but cannot be used directly from the backpack and do not receive numbered item planning tokens

#### Swapping Items
- **Usage:** During the hero's own activation, items may be swapped between the 6 active slots and the 3 backpack slots
- **Restriction:** Any item moved from the backpack into an active slot is **inactive until the next round**. It cannot be activated, committed with an item slot token, or provide passive bonuses before then
- **Restriction:** Any item moved out of an active slot immediately stops being usable as an active-slot item for the remainder of that activation

---

### Zone 4: Status Effects

Located at the bottom-left of the mat. Grid of status effect boxes with token placement areas.

#### Status Effect Icons
- **Component:** Printed icon grid with labeled boxes
- **Marker:** Colored token placed on active status effect
- **Duration Tracking:** Small number token (1–5) placed on status token if duration-based

**Status Effects Listed:**
| Icon | Effect | Duration Tracked? |
|------|--------|-------------------|
| ⚡ Stunned | AP penalty (see penalty value box) | Yes — rounds remaining |
| 🔇 Silenced | Cannot use abilities | Yes — rounds remaining |
| 🌿 Rooted | Cannot move | Yes — rounds remaining |
| ❄️ Slowed | Movement penalty | Yes — rounds remaining |
| 👁️ Invisible | Hidden from enemies | No (toggle) |
| 👻 Ethereal | Cannot attack/be attacked physically | Yes — rounds remaining |
| 🗡️ Disarmed | Cannot attack | Yes — rounds remaining |
| 💔 Broken | Passives disabled | No (toggle) |
| 🐸 Hexed | All abilities disabled | Yes — rounds remaining |
| 🩸 Bleeding/DoT | Damage over time | Yes — ticks remaining |
| 🛡️ BKB Active | Spell immunity | Yes — rounds remaining |

#### Stun Penalty Box
- **Component:** Printed box "AP Penalty: ___"
- **Marker:** D20 die or small numbered token showing AP loss value (e.g., 10, 15, 20)
- **Usage:** When stunned, place token showing exact AP penalty amount.

---

### Zone 5: Turn AP Tracker

Located at the very top, spanning the width of the mat.

#### AP Spent This Activation
- **Component:** Horizontal track with circles (0–10)
- **Marker:** Generic cube token tracking how many AP have been spent this turn
- **Usage:** Move token forward as actions are executed. Reset to 0 at start of each activation.

#### Reaction Slots
- **Component:** 2 printed slots to the left of the 10 action slots
- **Marker:** Standard planning tokens committed face-down
- **Usage:** During Planning Phase, place up to 2 reaction tokens here for the current half-round. Each committed reaction reserves 1 AP from that hero's normal AP budget and cannot also be committed to the hero's normal activation actions.

---

## Shared Game Board (Central Table)

Placed in the center of the table, visible to all players. Tracks global game state.

### Section 1: Round Structure

#### Round Counter
- **Component:** Large printed box "Round: ___"
- **Marker:** Two D10 dice showing round number (00–99, though games unlikely to exceed 30 rounds)

#### Half Tracker
- **Component:** Flip token (double-sided)
  - Front: "Turns 1–10 (Forward)"
  - Back: "Turns 11–20 (Backward)"
- **Usage:** Flip token at turn 10 to indicate second half of round.

#### Round Start Token
- **Component:** Large ornate token "⭐ FIRST PLAYER"
- **Usage:** Placed next to the hero standee of whichever hero activates first this round. Rotates to the next hero in sequence each round.

#### Turn Order Tracker
- **Component:** Printed vertical list with hero name slots (1–10 per side)
- **Usage:** Before game starts, write hero names in alternating team order (pendulum sequence). Reference throughout game.

---

### Section 2: Lanes

Three lane sections (Top, Mid, Bottom), each with identical tracking.

#### Creep Wave State (per lane)
- **Component:** Slide token with three positions
  - Normal (green)
  - Enhanced (yellow) — that lane's Barracks destroyed
  - Mega (red) — all 3 Barracks destroyed
- **Usage:** Move slider when Barracks are destroyed.

#### Creep Wave Exhausted (siege requirement)
- **Component:** Printed checkbox per lane "✓ Wave Exhausted This Round"
- **Marker:** Cube token placed when all enemy creep tokens in that lane have been removed for the round. Removed at Round End Phase.

#### Tower Health (per lane)
- **Component:** Printed tower icons (T1 → T2 → T3 → T4 × 2) with HP tracks
- **Marker:** Small cube token tracking current HP on each tower
- **Destroyed:** Place large red X token over tower icon when destroyed.

#### Barracks (per lane)
- **Component:** Printed broken-barracks art on the board beneath the lane's Barracks hex
- **Marker:** Removable standing Barracks token placed on top of that hex at game start
- **Usage:** Remove the standing Barracks token when the Barracks is destroyed.

---

### Section 3: Objectives

#### Roshan
- **Status:** Flip token (ALIVE / DEAD)
- **Respawn Countdown:** D6 die showing rounds until respawn (placed next to DEAD side)
- **HP During Fight:** Printed HP track (0–500) with cube token tracking current HP

#### Aegis of the Immortal
- **Component:** Printed box "Aegis on Board: ___"
- **Marker:** If dropped (not held by hero), place miniature Aegis token on the hex where it dropped. Include hex coordinates or descriptive location.

#### Power Rune
- **Type:** Place the matching Power Rune token in the designated box or on the rune hex
- **Location:** Coin placed on "Radiant Side" or "Dire Side" box
- **Claimed:** Checkbox with cube token (removed when rune is picked up)

---

### Section 4: Map State

#### Observer Wards
- **Component:** Printed grid "Observer Wards Placed"
  - Columns: Team | Hex Location | Duration Remaining
  - Rows: Up to 6 active wards per team
- **Marker:** Write hex coordinates with dry-erase marker (if using plastic overlay). Use a die or small generic number marker for duration countdown.

#### Sentry Wards
- **Component:** Same grid format as Observer Wards
- **Usage:** Identical tracking.

#### Courier
- **Position:** Miniature Courier standee placed on the board hex
- **Items Carried:** Item Cards placed beneath Courier standee on the board

#### Neutral Camps
- **Component:** Small tokens placed on each camp hex
  - Front: "Populated" (green)
  - Back: "Cleared" (gray)
- **Respawn:** Every even-numbered round, flip all cleared camps back to Populated.

#### Destroyed Trees
- **Component:** Remove Tree hex tokens when destroyed. Place small "Regrows Round ___" token with D6 die showing regrowth round number.
- **Regrowth:** Trees regrow every 4th round. Replace destroyed tree tokens at Round End Phase.

---

## Additional Physical Components

### Planning Tokens (Per Player)
A shared pool of reusable tokens used during the Planning Phase:
- **Move** tokens
- **Attack** tokens
- **Item Slot 1-6** tokens for the active item slots only
- **Pass** tokens
- **Hero Ability Tokens** (custom to each hero, one per named ability)

Players select tokens face-down during Planning Phase and place them in the Action Queue zone on their Hero Board.

---

### Token Summary

| Token Type | Color | Quantity Needed | Purpose |
|------------|-------|-----------------|---------|
| Small Cube | Assorted | 100+ | General-purpose tracking (cooldowns, statuses, checkboxes) |
| D6 Dice | Standard | 20+ | Charges, timers, XP progress |
| D10 Dice | Standard | 10+ | Round counter and general high-visibility numeric tracking |
| D20 Dice | Standard | 10+ | AP penalties, high-value counters |
| +1/+5/+10 Stat Tokens | Red/Gray/Green | 50+ | Attack/Defense/Move Speed bonuses |
| Hero Standee / Hero Token | Custom | 1 per hero | Represents the hero on the map and doubles as that hero's respawn marker when placed on a duration track after death |
| Status Effect Tokens | Colored Icons | 50+ | Stunned, Silenced, Rooted, etc. |
| Flip Tokens (Wards) | Green/Gray | 20+ | Populated or cleared camps |
| Aegis Token | Gold | 1 | Aegis item token and Aegis expiration marker when placed on a duration track |
| Buyback Token | Distinct Hero Marker | 1 per hero | Tracks Buyback cooldown when placed on the round cooldown track |
| Courier Delivery Token | Distinct Hero Marker | 1 per hero | Tracks when that hero's courier delivery arrives by sitting on a duration track |
| Round Start Token | Large Star | 1 | Marks first player each round |
| Courier Standee | Custom | 2 (1 per team) | Tracks the shared team Courier position on board |
| Power Rune Tokens | Custom | 5 | One token per rune type for river spawns and Bottle storage |
| Planning Tokens | Mixed | Per hero / per player set | Face-down action commitment during planning |

---

## Component Specifications

### Hero Board Material
- **Material:** Thick laminated cardboard (2mm) with glossy finish for durability
- **Size:** 30 × 40 cm (large enough to hold all zones without crowding)
- **Overlay Option:** Clear plastic sleeve allows dry-erase marker for temporary notes during prototyping, though the intended production version should rely primarily on tokens and the separate 3D-printed stat tracker

### Planning Tokens
- **Material:** Thick cardboard punchboard or acrylic tokens
- **Size:** 20-25 mm recommended for face-down handling
- **Faces:** Uniform back; front face shows the action or hero ability icon

### Tokens
- **Material:** Thick cardboard punchboard (1mm)
- **Size:** Small cubes (8mm), medium icons (15mm), large tokens (25mm)

### Dice
- **Standard D6, D10, D20** in multiple colors for easy differentiation

---

## Design Philosophy

1. **Visibility** — All critical information is immediately visible to the owning player and can be shared with opponents when needed through the board, tokens, cards, and the separate stat tracker.
2. **Uniformity** — The Hero Board remains generic across the full roster; hero-specific tracking should live on hero cards, ability cards, or dedicated tokens rather than requiring bespoke board layouts.
2. **Modularity** — Each tracking system is independent. Damage doesn't require recalculating multiple values.
3. **Minimal Writing** — Use dials, dice, and tokens instead of writing whenever possible to speed up gameplay.
4. **Redundancy Avoidance** — Don't track the same information in multiple places. Live numeric values belong on the separate stat tracker, while the Hero Board focuses on generic positional tracking surfaces.
5. **Accessibility** — Colorblind-friendly icons. Large text for readability. Tactile components (raised tokens, textured dice).

---

## Open Questions

- **XP Scaling:** If XP requirements vary significantly by level, consider a printed XP table with a sliding marker instead of a simple die.
- **Charge Items:** Should charge counters be universal (D6 for all items) or item-specific (custom dials)?
- **DoT Tracking:** Bleeding/DoT effects need both duration (ticks remaining) and damage value. Suggest a two-token system or small reference insert placed in Status Effects zone.
- **Ward Coordinates:** Hex notation (e.g., "D7") or descriptive locations (e.g., "Radiant jungle, near Ancient camp")? May need labeled hex grid on main board.

---

## Next Steps

1. **Prototype a Hero Board** — Print a mock layout at scale to validate zone sizing and token fit.
2. **Test tracking flow** — Simulate a full turn with Sven to ensure all interactions (ability use, item use, status effects, cooldown timing, courier timing, and death / respawn handling) are smooth.
3. **Refine token counts** — Playtest to determine if 100 small cubes is sufficient or if more are needed.
4. **Finalize shared board layout** — Integrate lane tracking, Roshan, and runes into the main game board or separate tracking mat.
