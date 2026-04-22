# DOTA 2: THE BOARD GAME — HERO BOARD LAYOUT & TRACKING SYSTEM

This document specifies how all game variables are tracked using physical, offline components: cardboard mats, tokens, dice, sliders, and cards. No companion apps, no digital tracking — everything is tactile and visible.

**Measurement Note:** Use the metric system for all physical component specifications in this project.

---

## Individual Hero Board (Player Mat)

Each player receives a **Hero Board** — a large printed cardboard mat (approximately 30 × 40 cm) that holds all information for one hero. The board is divided into functional zones.

### Zone 1: Base Stats & Resources

Located at the top of the mat. Uses **3D-printed number trackers** for HP, Mana, and Level tracking.

#### HP Track
- **Component:** 3D-printed multi-digit number tracker ([Thingiverse #3458256](https://www.thingiverse.com/thing:3458256))
  - Current HP tracker (red or primary color)
  - Max HP tracker (white or secondary color, starts at hero's base HP)
- **Scale:** 0–999 (adjustable digits)
- **Usage:** Rotate digit wheels to display current HP and max HP. Update current HP as damage is taken/healed. Update max HP when it increases via leveling or items.

#### Mana Track
- **Component:** 3D-printed multi-digit number tracker ([Thingiverse #3458256](https://www.thingiverse.com/thing:3458256))
  - Current Mana tracker (blue or primary color)
  - Max Mana tracker (white or secondary color)
- **Scale:** 0–999 (adjustable digits)
- **Usage:** Rotate digit wheels to display current Mana and max Mana. Update current Mana as mana is spent/restored. Update max Mana when it increases via leveling or items.

#### Static Stats Display
- **Component:** Printed boxes with **stackable +1 tokens** for modifications
- **Stats displayed:**
  - **Attack** — Base value printed. Add red +1/+5/+10 tokens for item/buff bonuses.
  - **Defense** — Base value printed. Add gray +1/+5 tokens for item/buff bonuses.
  - **Move Speed** — Base value printed. Add green +1 tokens for item/buff bonuses.
  - **AP per Turn** — Base value printed. Stun penalties tracked separately (see Status Effects).

---

### Zone 2: Progression & Leveling

Located in the upper-right corner.

#### Level Track
- **Component:** 3D-printed multi-digit number tracker ([Thingiverse #3458256](https://www.thingiverse.com/thing:3458256))
- **Scale:** 1–18 (or up to 99 with two digits)
- **Usage:** Rotate digit wheels to display current hero level. Check ability unlock milestones at levels 6, 12, and 18.

#### XP Counter
- **Component:** Printed XP threshold table + **6-sided die** placed next to it
- **Scale:** 0–5 on the die (represents partial progress toward next level)
- **Usage:** Rotate die face to show XP progress. When die reaches 6, level up and reset die to 1.

#### Ability Unlock Tracker
- **Component:** Three checkboxes printed on the mat
  - ☐ Level 6 — Ultimate Unlocked
  - ☐ Level 12 — Ultimate Upgraded
  - ☐ Level 18 — Ultimate Max Level
- **Usage:** Check visually against the hero's current Level tracker; no dedicated milestone token is required.

---

### Zone 3: Action Planning & Duration Tracking

Located in the center of the mat. This zone serves two purposes: staging face-down planning tokens for the current turn and tracking all time-based effects.

#### Planning Token Staging Area
Located at the top of Zone 3.

- **Component:** Rectangular zone labeled "Action Queue"
- **Size:** Fits up to 10 planning tokens laid horizontally in sequence
- **Usage:** During Planning Phase, place selected tokens face-down here in the order you want to execute them. During your activation, reveal and execute from left to right.

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

---

#### Additional Ability Tracking (Optional)

For heroes with abilities requiring special tracking (stacks, charges, channeling):

**Ability Stacks**
- **Component:** Small printed box at the bottom of Zone 3 labeled "Ability Stacks: ___"
- **Marker:** D20 die or small numbered dial (0–20)
- **Usage:** For abilities like Flesh Heap (Pudge), Essence Shift (Slark), Fervor (Ursa) — track permanent or temporary stacks.

**Channeling Indicator**
- **Component:** Hourglass token placed on relevant ability identifier in the Action Queue or Cooldown sections
- **Usage:** Indicates ability is being channeled and can be interrupted.

---

### Zone 4: Item Slots (×6)

Located in the center-right of the mat. Six horizontal item slots arranged vertically.

#### Item Card Slot
- **Component:** Standard card slot (fits Item Cards)
- **Card displays:** Item name, stats/bonuses, active effect (if any)

#### Per-Item Tracking (printed beside each slot)
- **Active Cooldown:**
  - Small circles: 0 ← 1 ← 2 ← 3 rounds
  - Marker: Small cube token (same system as ability cooldowns)
  
- **Charge Counter:**
  - Printed box: "Charges: ___"
  - Component: D6 die or small numbered token (0–6)
  - Usage: For items like Magic Wand, Urn of Shadows, Spirit Vessel, Drum of Endurance

---

### Zone 5: Status Effects

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

### Zone 6: Economy

Located at the bottom-center of the mat.

#### Gold Counter
- **Component:** Printed box "Gold: _____"
- **Marker:** Two D10 dice (showing tens and ones, allowing 00–99 range)
- **Alternative:** Three D10 for 0–999 if gold values are higher
- **Usage:** Rotate dice to display current gold total.

#### Passive Income
- **Component:** Printed box "Income/Round: ___"
- **Marker:** Static printed value or small numbered token (updated if passive income changes)

#### Courier Delivery Timer
- **Component:** Printed box "Courier ETA: ___ rounds"
- **Marker:** D6 die or small numbered token (0–5)
- **Usage:** Place die showing rounds until courier delivers items.

---

### Zone 7: Alive/Dead & Respawn

Located at the bottom-right of the mat.

#### Alive/Dead Indicator
- **Component:** Flip token (double-sided)
  - Front: ✓ ALIVE (green)
  - Back: ✗ DEAD (red)
- **Usage:** Flip token when hero dies.

#### Respawn Counter
- **Component:** Printed box "Respawn in: ___ turns"
- **Marker:** D20 die or small numbered token (0–20 turns, scales with level)
- **Usage:** When dead, place die showing respawn countdown. Decrement each turn.

#### Buyback Tracker
- **Component:** Dedicated Buyback token + printed ready space beside the hero board's round cooldown track
- **Marker:** The Buyback token sits in its ready space while available.
- **Usage:** When Buyback is used, move the Buyback token into the round cooldown track at its cooldown value. Advance it toward 0 during Round End updates, just like other round-based cooldown pieces. When it reaches 0, return it to the ready space.

#### Aegis Held
- **Component:** Printed checkbox "🛡️ Aegis of the Immortal"
- **Marker:** Aegis token (large, ornate) placed on checkbox when hero holds Aegis
- **Usage:** When hero dies with Aegis, remove Aegis token and flip Alive/Dead token back to ALIVE.

---

### Zone 8: Aghanim's Scepter

Located near the hero's Abilities Card reference area.

#### Scepter Acquired
- **Component:** Printed checkbox "⭐ Aghanim's Scepter"
- **Marker:** Star token placed when Scepter is purchased
- **Usage:** The item in the inventory slot already makes Scepter ownership visible, so this token functions only as a quick hero-board reminder. No separate upgrade pointer is needed because the upgraded ability is printed directly on the Abilities Card.

---

### Zone 10: Turn AP Tracker

Located at the very top, spanning the width of the mat.

#### AP Spent This Activation
- **Component:** Horizontal track with circles (0–10)
- **Marker:** Generic cube token tracking how many AP have been spent this turn
- **Usage:** Move token forward as actions are executed. Reset to 0 at start of each activation.

#### Reaction AP Owed
- **Component:** Printed box "Reaction AP Debt: ___"
- **Marker:** Small numbered token (1–5)
- **Usage:** When spending AP from next turn for a Reaction (e.g., Deny), place token showing how much AP is deducted from next activation.

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
  - Enhanced / Super (yellow) — one Barracks destroyed
  - Mega (red) — both Barracks destroyed
- **Usage:** Move slider when Barracks are destroyed.

#### Creep Wave Exhausted (siege requirement)
- **Component:** Printed checkbox per lane "✓ Wave Exhausted This Round"
- **Marker:** Cube token placed when creeps have been farmed. Removed at Round End Phase.

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
- **Farm** tokens
- **Use Item** tokens
- **Pass** tokens
- **Hero Ability Tokens** (custom to each hero, one per named ability)

Players select tokens face-down during Planning Phase and place them in the Action Queue zone on their Hero Board.

---

### Token Summary

| Token Type | Color | Quantity Needed | Purpose |
|------------|-------|-----------------|---------|
| Small Cube | Assorted | 100+ | General-purpose tracking (cooldowns, statuses, checkboxes) |
| D6 Dice | Standard | 20+ | Charges, timers, XP progress |
| D10 Dice | Standard | 10+ | Gold counter, round counter |
| D20 Dice | Standard | 10+ | AP penalties, high-value counters |
| +1/+5/+10 Stat Tokens | Red/Gray/Green | 50+ | Attack/Defense/Move Speed bonuses |
| Hero Standee | Custom | 1 per hero | Marks level on Hero Board, represents hero on map |
| Status Effect Tokens | Colored Icons | 50+ | Stunned, Silenced, Rooted, etc. |
| Flip Tokens (Alive/Dead) | Green/Red | 1 per hero | Alive or dead status |
| Flip Tokens (Wards) | Green/Gray | 20+ | Populated or cleared camps |
| Aegis Token | Gold | 1 | Aegis of the Immortal holder |
| Round Start Token | Large Star | 1 | Marks first player each round |
| Courier Standee | Custom | 2 (1 per team) | Tracks Courier position on board |
| Power Rune Tokens | Custom | 5 | One token per rune type for river spawns and Bottle storage |
| Planning Tokens | Mixed | Per hero / per player set | Face-down action commitment during planning |

---

## Component Specifications

### Hero Board Material
- **Material:** Thick laminated cardboard (2mm) with glossy finish for durability
- **Size:** 30 × 40 cm (large enough to hold all zones without crowding)
- **Overlay Option:** Clear plastic sleeve allows dry-erase marker for dynamic values (gold, timers, ward locations)

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

1. **Visibility** — All critical information is immediately visible to the owning player and can be shared with opponents when needed (HP, status effects, gold).
2. **Modularity** — Each tracking system is independent. Damage doesn't require recalculating multiple values.
3. **Minimal Writing** — Use dials, dice, and tokens instead of writing whenever possible to speed up gameplay.
4. **Redundancy Avoidance** — Don't track the same information in multiple places. Max HP lives on the Hero Board only, not on a separate sheet.
5. **Accessibility** — Colorblind-friendly icons. Large text for readability. Tactile components (raised tokens, textured dice).

---

## Open Questions

- **XP Scaling:** If XP requirements vary significantly by level, consider a printed XP table with a sliding marker instead of a simple die.
- **Charge Items:** Should charge counters be universal (D6 for all items) or item-specific (custom dials)?
- **DoT Tracking:** Bleeding/DoT effects need both duration (ticks remaining) and damage value. Suggest a two-token system or small reference insert placed in Status Effects zone.
- **High Gold Values:** If late-game gold exceeds 999, consider using poker chips (10/50/100 denominations) instead of dice.
- **Ward Coordinates:** Hex notation (e.g., "D7") or descriptive locations (e.g., "Radiant jungle, near Ancient camp")? May need labeled hex grid on main board.

---

## Next Steps

1. **Prototype a Hero Board** — Print a mock layout at scale to validate zone sizing and token fit.
2. **Test tracking flow** — Simulate a full turn with Sven to ensure all interactions (leveling, ability use, item purchase, status effects) are smooth.
3. **Refine token counts** — Playtest to determine if 100 small cubes is sufficient or if more are needed.
4. **Finalize shared board layout** — Integrate lane tracking, Roshan, and runes into the main game board or separate tracking mat.
