# Token Asset Prompt Draft

This document is a first-pass grouping plan for token art generation pages.

The goal is to cluster tokens that can share one image-generation page because they belong to the same visual family, use a similar production scale, or benefit from being designed as a matching set.

This draft does **not** contain final image prompts yet. It only groups token families for later prompt writing.

---

## Grouping Principles

- Group tokens that should share a common frame, border, icon system, or color language.
- Separate tokens that need different physical scale, readability distance, or hidden-information treatment.
- Keep page groupings broad enough to save generations, but narrow enough that the art model does not drift into mixed visual logic.
- Prefer one page per reusable token family rather than one page per individual token where possible.

---

## Page Group 1: Core Hero And Unit Presence

These are the main board-presence pieces that represent units or moving actors on the map.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Hero Presence | Hero Tokens | All hero board-presence pieces need the same readable top-down or standee-style visual language. |
| Allied Utility Unit Presence | Courier Token | Courier should feel like part of the same map-piece family as heroes and illusions. |
| Temporary Unit Presence | Illusion Tokens | Illusions should clearly echo hero presence while remaining visually distinct. |

---

## Page Group 2: Lane, Camp, And Neutral Board Counters

These are small board counters that track non-hero units and map-state occupancy.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Lane Wave Counters | Lane Creep Tokens / Counters | Shared small-counter language for repeatable board states. |
| Neutral Camp Counters | Neutral Camp Tokens / Counters | Uses the same production logic as lane creeps, but with neutral-specific identity. |
| Ancient Camp Counters | Ancient Camp Tokens / Counters | Best treated as the elite variant of neutral camp counters. |
| Camp Availability | Camp Cleared / Populated Marker | Tracks the same neutral ecosystem and should match the camp counter set. |

---

## Page Group 3: Structural Objectives And Destruction States

These tokens represent buildings, lane collapse, and large strategic map states.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Tower Destruction | Tower Destroyed Marker | Large overlay marker for destroyed structures. |
| Barracks Presence | Barracks Status Marker | Standing Barracks tokens should be designed as removable single-hex board pieces. |

---

## Page Group 4: Roshan And Major Objective Rewards

These tokens center on Roshan and premium objective-state pieces.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Roshan Encounter | Roshan Alive / Dead Marker | Roshan's state still needs a dedicated premium objective marker. |
| Premium Objective Reward | Aegis of the Immortal Token | Aegis should be designed in the same premium objective language as Roshan tracking. |

---

## Page Group 5: Rune System And Stored Rune States

These tokens all belong to the rune ecosystem and should share iconography.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Spawned Rune Presence | Power Rune Tokens | Generate all five single-hex rune tokens as one coherent symbol family. |

---

## Page Group 6: Vision, Detection, And Hidden Information Tokens

These tokens interact with warding, revelation, and secret positioning. They should be designed together so their front-facing information system is coherent.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Ward Placement | Observer Ward Token, Sentry Ward Token | These are the core vision pieces and need a shared ward language. |

### Keep Separate Within The Same Future Prompt Set

- Invisibility Cloud Token
- Smoke Cloud Token

These two should likely share an overall hidden-positioning art direction, but they may need their own page or sub-prompt because they are larger template-like pieces rather than compact ward markers.

---

## Page Group 7: Round Flow And Turn Order Helpers

These are compact system markers used to track round structure rather than hero state.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Turn Order | Round Start Token | Shared game-flow marker language. |
| Round Phase | Half-Round Marker | Same table-utility family as round start tracking. |

---

## Page Group 8: Shared Action Planning Tokens

These are the universal planning tokens used by every hero.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Core Action Commitments | Move, Attack, Pass | All three must read as a single hidden-planning product set. |

---

## Page Group 9: Item Planning Token Set

These are a numbered system and should be designed as one page.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Item Slot Commitments | Item Slot 1 Token, Item Slot 2 Token, Item Slot 3 Token, Item Slot 4 Token, Item Slot 5 Token, Item Slot 6 Token | This is one strict numbered family with shared frame and slot identity. |

---

## Page Group 10: Hero Ability Planning Template

These tokens are hero-specific, but their shared structure should be established as one template family before individual hero pages are written.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Ability Planning Frame | Ability 1 Token, Ability 2 Token, Ability 3 Token, Ultimate Token | All heroes should inherit the same planning-token architecture, with hero-specific icon swaps later. |

### Note

This page should define the common frame system only. Individual hero prompt pages can later plug in iconography and color accents per hero.

---

## Page Group 11: Core Status Effects

These are the universal condition markers most likely to appear across heroes and items.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Hard Control | Stunned, Hexed, Silenced, Rooted, Disarmed, Broken | These are all high-priority negative status markers. |
| State And Vulnerability | Slowed, Ethereal, Invisible, Bleeding / DoT, BKB Active / Spell Immunity | These are common state-change markers that need a consistent buff/debuff language. |

---

## Page Group 12: Generic Hero Board Tracking Markers

These tokens track time, cooldown, AP, life state, and progression on Hero Boards.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Cooldown Identity | Ability Identifier Tokens | These sit in printed cooldown tracks and need a consistent visual system. |
| Activation State | Channeling Token | Channeling still benefits from a dedicated state token. |
| Life Cycle | Alive / Dead Flip Token, Buyback Token | These are the remaining dedicated death-cycle tokens. |
| Progression State | Scepter Acquired Token | Scepter remains a visible board-state reminder if a separate token is kept in production. |

---

## Page Group 13: Numeric Stat Modification Set

These are modular number-adjustment tokens and should be generated together as one arithmetic family.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Attack Modifiers | +1 Attack Token, +5 Attack Token, +10 Attack Token | Shared plus-value visual system. |
| Defense Modifiers | +1 Defense Token, +5 Defense Token | Same numeric stat-boost family. |
| Mobility Modifiers | +1 Move Speed Token | Fits the same stat-modifier design language. |

---

## Page Group 14: Economy, Drops, And Charge Tracking

These tokens handle item drops, economy reminders, and generic consumable counters.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Dropped Artifact State | Gem of True Sight Drop Token, Divine Rapier Drop Token | Both represent valuable items dropped onto the board. |

---

## Page Group 15: Rune Buffs And Temporary Hero Buff States

These are hero-affecting buff markers that come from runes or closely related temporary effects.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Rune Buff States | Haste Marker, Regeneration Marker, Double Damage Marker | These should be one coherent buff set tied directly to rune iconography. |

---

## Page Group 16: Item Effect Marker Library

These are reusable item-derived status and shield markers. They should be generated as a broad matching library rather than as isolated one-offs.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Defensive Triggers | Shield Token, Magic Barrier Token, Physical Block Token, Static Shield Token, Aeon Shield Token | All represent defensive prevention or retaliation states. |
| Reflection And Amplification | Lotus Echo Token, Veil Token | Both represent high-clarity effect modifiers that sit on a target. |
| Suppression And Debuff | Nullify Token, Arctic Slow Token, Slow Token, Silence Token, Hex Token | These are shared item-to-hero condition markers. |
| Delayed Resolution | Magic Damage Counter Token | Belongs to the same item-effect library and should match its visual logic. |

---

## Page Group 17: Hidden Position Templates

These are larger positional concealment pieces and should be treated as their own template page.

| Token Family | Include On This Page | Why They Belong Together |
|---|---|---|
| Single-Hero Hidden Position | Invisibility Cloud Token | Template-style hidden position piece. |
| Multi-Hero Hidden Position | Smoke Cloud Token | Larger concealment template in the same family. |

---

## Page Group 18: Future Bespoke Hero Mechanics

These should not be mixed into shared generic pages until the specific hero mechanics are defined.

| Future Family | Hold For Later |
|---|---|
| Summoned units | One hero-specific page family per mechanic cluster |
| Trap or mine tokens | One hero-specific page family per mechanic cluster |
| Remnant or spirit tokens | One hero-specific page family per mechanic cluster |
| Stack counters for scaling passives | Can later merge into a shared stack-counter library if enough overlap appears |
| Orbiting shield or charge markers | Keep separate until multiple heroes share the pattern |
| Zone templates for persistent spell areas | Template page family, likely separate from compact tokens |
| Transformation state markers | One hero-specific subfamily or transformation library |

---

## Recommended Generation Order

If asset production starts soon, the most efficient first batch is:

1. Shared Action Planning Tokens
2. Item Planning Token Set
3. Core Status Effects
4. Generic Hero Board Tracking Markers
5. Rune System And Stored Rune States
6. Vision, Detection, And Hidden Information Tokens
7. Lane, Camp, And Neutral Board Counters
8. Structural Objectives And Destruction States

These pages cover the largest number of reusable tokens while establishing the core icon language for the full set.