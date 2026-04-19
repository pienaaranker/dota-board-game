# DOTA 2: THE BOARD GAME — HERO BOARD LAYOUT & TRACKING SYSTEM

This document specifies how all game variables are tracked using physical, offline components: cardboard mats, tokens, dice, sliders, and cards. No companion apps, no digital tracking — everything is tactile and visible.

---

## Individual Hero Board (Player Mat)

Each player receives a **Hero Board** — a large printed cardboard mat (approximately 12"×16") that holds all information for one hero. The board is divided into functional zones.

### Zone 1: Base Stats & Resources

Located at the top of the mat. Uses **dual-track sliders** for current/max values.

#### HP Track
- **Component:** Dual slider with two movable markers
  - Inner track: Current HP (red marker)
  - Outer track: Max HP (white marker, starts at hero's base HP)
- **Scale:** 0–300 in increments of 5
- **Usage:** Move red marker as damage is taken/healed. Move white marker when max HP increases via leveling or items.

#### Mana Track
- **Component:** Dual slider with two movable markers
  - Inner track: Current Mana (blue marker)
  - Outer track: Max Mana (white marker)
- **Scale:** 0–200 in increments of 5
- **Usage:** Move blue marker as mana is spent/restored. Move white marker when max Mana increases via leveling or items.

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
- **Component:** Vertical track with numbered circles (1–18)
- **Marker:** Hero standee token placed on current level
- **Special markers:** Stars printed at levels 6, 12, and 18 (ability unlock milestones)

#### XP Counter
- **Component:** Printed XP threshold table + **6-sided die** placed next to it
- **Scale:** 0–5 on the die (represents partial progress toward next level)
- **Usage:** Rotate die face to show XP progress. When die reaches 6, level up and reset die to 1.

#### Ability Unlock Tracker
- **Component:** Three checkboxes printed on the mat
  - ☐ Level 6 — Ultimate Unlocked
  - ☐ Level 12 — Ultimate Upgraded
  - ☐ Level 18 — Ultimate Max Level
- **Marker:** Place small cube token on checked box when milestone is reached.

---

### Zone 3: Ability Cards (×4 slots)

Located in the center-left of the mat. Four horizontal card slots, each with printed tracking beneath.

#### Ability Card Slot
- **Component:** Standard card slot (fits Hero Ability Cards)
- **Card displays:** Ability name, type, mana cost, effect description

#### Per-Ability Tracking (printed beneath each slot)
- **Cooldown Track:**
  - Printed circles: 0 ← 1 ← 2 ← 3 ← 4 ← 5 rounds
  - Marker: Small cube token placed on current cooldown value
  - Usage: After using ability, place token on cooldown length. Move one step toward 0 each round.
  
- **Channeling Indicator:**
  - Printed checkbox: "⏳ Channeling"
  - Marker: Hourglass token placed on checkbox when channeling active

- **Stack Counter (for stackable abilities):**
  - Printed box: "Stacks: ___"
  - Component: D20 die or small numbered dial (0–20)
  - Usage: For abilities like Flesh Heap, Essence Shift — track permanent stacks per hero or global.

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
- **Component:** Printed checkbox "💰 Buyback Available"
- **Marker:** Cube token placed when buyback is available, removed when used
- **Last Used:** Small number token placed in "Last Buyback: Round ___" box

#### Aegis Held
- **Component:** Printed checkbox "🛡️ Aegis of the Immortal"
- **Marker:** Aegis token (large, ornate) placed on checkbox when hero holds Aegis
- **Usage:** When hero dies with Aegis, remove Aegis token and flip Alive/Dead token back to ALIVE.

---

### Zone 8: Aghanim's Scepter

Located near the ability cards.

#### Scepter Acquired
- **Component:** Printed checkbox "⭐ Aghanim's Scepter"
- **Marker:** Star token placed when Scepter is purchased
- **Upgraded Ability:** Small arrow token points to which ability is upgraded (if not obvious from card)

---

### Zone 9: Action Planning Staging Area

Located at the top-right corner, separate from other zones.

#### Face-Down Action Cards
- **Component:** Designated rectangle "Action Queue (Face-Down)"
- **Usage:** During Planning Phase, place selected Action Cards face-down here in order. Reveal and execute during activation.
- **Size:** Fits up to 10 Action Cards (max AP)

---

### Zone 10: Turn AP Tracker

Located at the very top, spanning the width of the mat.

#### AP Spent This Activation
- **Component:** Horizontal track with circles (0–10)
- **Marker:** Cube token tracking how many AP have been spent this turn
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
- **Component:** Printed Barracks icon per lane
- **Marker:** Flip token (Alive / Destroyed)

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
- **Type:** Custom Rune Die placed in designated box (shows which rune spawned)
- **Location:** Coin placed on "Radiant Side" or "Dire Side" box
- **Claimed:** Checkbox with cube token (removed when rune is picked up)

---

### Section 4: Map State

#### Observer Wards
- **Component:** Printed grid "Observer Wards Placed"
  - Columns: Team | Hex Location | Duration Remaining
  - Rows: Up to 6 active wards per team
- **Marker:** Write hex coordinates with dry-erase marker (if using plastic overlay). Use small numbered token for duration countdown.

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

### Action Cards (Per Player)
A deck of reusable Action Cards used during the Planning Phase:
- **Move** (×10)
- **Attack** (×10)
- **Farm** (×5)
- **Use Ability** (×10, labeled Ability 1–4 or generic "Use Ability")
- **Use Item** (×10, labeled Slot 1–6 or generic "Use Item")
- **Pass** (×5)

Players select cards face-down during Planning Phase and place them in the Action Queue zone on their Hero Board.

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
| Rune Die | Custom | 1 | Determines which Power Rune spawns |

---

## Component Specifications

### Hero Board Material
- **Material:** Thick laminated cardboard (2mm) with glossy finish for durability
- **Size:** 12"×16" (large enough to hold all zones without crowding)
- **Overlay Option:** Clear plastic sleeve allows dry-erase marker for dynamic values (gold, timers, ward locations)

### Action Cards
- **Material:** Standard playing card stock with linen finish
- **Size:** Poker-sized (2.5"×3.5")
- **Backs:** Uniform design (no information, face-down during Planning)

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
- **DoT Tracking:** Bleeding/DoT effects need both duration (ticks remaining) and damage value. Suggest a two-token system or small card placed in Status Effects zone.
- **High Gold Values:** If late-game gold exceeds 999, consider using poker chips (10/50/100 denominations) instead of dice.
- **Ward Coordinates:** Hex notation (e.g., "D7") or descriptive locations (e.g., "Radiant jungle, near Ancient camp")? May need labeled hex grid on main board.

---

## Next Steps

1. **Prototype a Hero Board** — Print a mock layout at scale to validate zone sizing and token fit.
2. **Test tracking flow** — Simulate a full turn with Sven to ensure all interactions (leveling, ability use, item purchase, status effects) are smooth.
3. **Refine token counts** — Playtest to determine if 100 small cubes is sufficient or if more are needed.
4. **Finalize shared board layout** — Integrate lane tracking, Roshan, and runes into the main game board or separate tracking mat.
