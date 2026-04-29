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
| Lane Wave Counters | Melee Lane Creep Tokens (double-sided 2-creep / 1-creep), Ranged Lane Creep Tokens | Shared small-counter language for repeatable lane states, with the melee family built as a reversible damage-state token. |
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
| Shared Damage State | Creep Damage Marker | Small generic marker placed on Super and Mega lane creep tokens to show the current front-most creep has lost 1 Hit. |
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

---

## Final Prompt Draft — Board Presence And Vision Token Sheet

Use the following prompt when generating the first printable token sheet for **board presence / objective tokens** and **compact vision tokens**.

This prompt assumes two attachments are supplied to the image model:

- **Attachment 1:** the token-sheet layout wireframe with the large top section and smaller bottom section
- **Attachment 2:** the Rubick hero card image used only as a **style-family reference**, not as subject matter

```text
Create a flat, print-ready fantasy board game token sheet that follows the attached wireframe layout exactly.

This is a premium tabletop component for a Dota-inspired board game. The result must look like it belongs to the same manufactured product family as the attached Rubick hero card, but it must not copy that card's specific character art, Rubick iconography, or hero-specific symbols. Use the Rubick card only as a style reference for material finish, border treatment, palette discipline, ornament density, typography mood, and icon rendering quality.

PRIMARY GOAL
Generate a clean printable token sheet for:
1. Board Presence And Objective Tokens
2. Vision, Hidden Information, And Deception Tokens

LOCKED LAYOUT REQUIREMENTS
- Preserve the attached token-sheet page layout exactly.
- Keep the same page proportions, same large rounded outer border, same inner section boxes, same section-title placement, and the same arrangement of rotated rounded-square token cut zones.
- Keep the top section as the larger area labeled Board Presence And Objective Tokens.
- Keep the bottom section as the smaller area labeled Vision, Hidden Information, And Deception Tokens.
- Keep the token cells aligned exactly to the wireframe grid.
- Do not redesign the page architecture.
- Do not change the number, spacing, tilt, or proportions of the token slots.
- Present the page straight-on, perfectly flat, with no perspective distortion.

PRINTABILITY REQUIREMENTS
- This must read as a real printable token sheet, not a mockup.
- Use a bright clean background suitable for printing.
- Keep all token art fully contained inside its own token boundary.
- Leave clean gutters between token cells for cutting or punchboard separation.
- Use crisp outlines and high-contrast iconography.
- Avoid muddy shadows, fog, overpainting, or low-contrast effects that would reduce print legibility.
- Do not place hands, table surfaces, props, scissors, dice, cards, rulers, or environmental scene dressing around the page.
- Do not render the page as a photographed object, angled sheet, curled poster, or 3D product mockup.
- No dramatic cast shadows outside the token artwork.
- No fake paper texture so heavy that it interferes with token readability.

STYLE DIRECTION
- Match the general visual sophistication of the attached Rubick hero card.
- Use the same overall product-family feeling: polished fantasy board game component, restrained premium ornament, elegant gold-edged detailing, dark teal / deep green / navy structural tones, ivory highlights, and crisp readable icon-first design.
- Do not make this token sheet Rubick-themed. The palette and ornament system should feel like the same publisher and same component line, not like a Rubick expansion sheet.
- Let each token family use its own color-coded icon treatment inside that shared system.
- The tokens should feel readable at arm's length on a real tabletop.

TOKEN FRAME SYSTEM
- Every token should use the same manufactured frame language.
- Each token should have a consistent border treatment that feels related to the hero card frame: thin premium border, subtle inner panel, and a strong central icon area.
- Keep the token faces clean and icon-forward.
- Minimal or no text on token faces unless absolutely necessary.
- If text is used at all, it must be tiny, secondary, and never dominate the token.

TOP SECTION CONTENT: BOARD PRESENCE AND OBJECTIVE TOKENS
The top section should contain compact board tokens from these families:
- lane creep
- neutral camp
- ancient camp
- barracks standing marker
- Roshan marker
- Aegis of the Immortal
- power rune set: Illusion, Haste, Invisibility, Regeneration, Double Damage
- courier
- broken tree

Do NOT include hero portrait tokens on this sheet.
Do NOT include Ancient or Tower position markers, because those should be printed on the board rather than manufactured as tokens.

BOARD TOKEN VISUAL RULES
- Melee lane creep token: simple hostile lane-unit iconography, readable, faction-neutral, mass-produced feel. This family must support a double-sided 2-creep / 1-creep state.
- Ranged lane creep token: matching lane-unit family, but clearly the rear support creep rather than a front-line melee body.
- Neutral camp token: beast / fang / claw / horn language, clearly different from lane creeps.
- Ancient camp token: elite neutral treatment, heavier silhouette, more dangerous and ancient-looking than standard neutral camp tokens.
- Barracks token: structural fortified building icon, readable as a standing objective.
- Roshan token: premium boss marker, heavier visual weight than all other board tokens.
- Aegis token: premium relic look, gold and sacred aura, clearly a high-value objective reward.
- Power rune tokens: one full coherent 5-token set with distinct icons and color coding:
	- Illusion: spectral or mirrored motif
	- Haste: motion / wind / streak motif
	- Invisibility: eye-hidden / haze / veil motif
	- Regeneration: restorative life / leaf / healing-water motif
	- Double Damage: explosive / crossed-strike / radiant impact motif
- Courier token: allied utility piece, messenger silhouette, readable and distinct from combat units.
- Broken tree token: a cut stump / broken trunk / exposed roots motif that clearly signals a once-blocked space now opened.

TOP SECTION REPETITION PRIORITY
Repeat token types to fill the available slots, prioritizing the tokens that need multiple copies in actual play.
Use this duplication priority from highest to lowest:
1. broken tree
2. lane creep
3. neutral camp
4. barracks
5. courier
6. ancient camp
7. power runes
8. Roshan
9. Aegis

BOTTOM SECTION CONTENT: COMPACT VISION TOKENS
The bottom section should contain only compact vision tokens:
- Observer Ward
- Sentry Ward

Do NOT include Invisibility Cloud or Smoke Cloud on this sheet.
Those are larger hidden-position templates and should be generated as separate assets later.

VISION TOKEN VISUAL RULES
- Observer Ward: elegant watchful vision iconography, mystical but non-aggressive, intelligence / sight / awareness theme.
- Sentry Ward: same family as Observer Ward but clearly distinct through sharper detection / reveal / true-sight language.
- The two ward types must feel manufactured as a matching pair.
- They should be instantly distinguishable from each other even when viewed from across the table.

BOTTOM SECTION REPETITION RULE
- Fill the bottom section primarily with Observer Ward and Sentry Ward tokens.
- Keep both types repeated multiple times in balanced proportion.
- Slightly favor Observer Wards if an uneven count is needed.

ICONOGRAPHY RULES
- Use bold central symbols with clean silhouettes.
- Favor icon clarity over painterly detail.
- Use subtle magical embellishment, not noisy illustrative clutter.
- Keep token identity understandable even if printed small.
- No token should depend on tiny text to be recognized.

ANTI-DRIFT / NEGATIVE CONSTRAINTS
- Do not redesign the page layout.
- Do not change the token slot arrangement.
- Do not turn the sheet into cards, stickers, coins photographed on a table, or a punchboard mockup seen at an angle.
- Do not include Rubick himself, his staff, his face, or his spell icons as token subjects.
- Do not use copyrighted Dota 2 UI symbols or official Valve art.
- Do not make the tokens muddy, hyper-rendered, or overloaded with effects.
- Do not place giant text labels inside each token.
- Do not add extra token categories not listed above.
- Do not include hero tokens, invisibility clouds, smoke clouds, or planning tokens on this page.

FINAL OUTPUT TARGET
The final image should look like a production-quality printable token sheet for a premium fantasy board game: clean, aligned, readable, stylistically cohesive with the attached Rubick hero card, and immediately usable as a print reference for board presence and ward tokens.
```

## Practical Note

This prompt intentionally excludes **hero tokens**, **Invisibility Cloud**, and **Smoke Cloud** from the sheet even though they belong to nearby token families. They need different scale and layout treatment than the compact token grid shown in the attached wireframe.