# DOTA 2: THE BOARD GAME — TOKENS

This document is the master list of all tokens and token-like markers that need visual design and production planning for the game.

Its purpose is to answer two questions:
- Which physical tokens must exist on the table or Hero Boards during play?
- Which token families must be supported as the hero roster and item pool expand?

This document focuses on **tokens and markers**. It does **not** cover full cards, dice, dials, or 3D number trackers unless a token is still needed alongside them.

---

## Token Design Principles

- Tokens should be readable from across the table.
- Team ownership must be instantly clear for all board tokens.
- Temporary effects should use a consistent icon language across heroes and items.
- Hidden-information tokens must have uniform backs where required.
- Shared marker tokens should be reusable across many systems whenever possible.
- If a rule can be tracked with one generic marker plus a number token, prefer that over creating a unique token for every edge case.

---

## 1. Core Board Tokens

These are the tokens required to run the map, objectives, lane pressure, and board-state systems.

| Token | Purpose | Notes |
|---|---|---|
| **Hero Tokens** | Represent hero position on the board | One token per drafted hero, team-colored or team-rimmed. |
| **Lane Creep Tokens / Counters** | Represent lane creeps at each Creep Meeting Point | Should support normal lane state and removal through Farm. |
| **Neutral Camp Tokens / Counters** | Represent remaining neutral creeps in a camp | Used for camp farming and respawn tracking. |
| **Ancient Camp Tokens / Counters** | Represent remaining Ancient creeps in a camp | Visually distinct from regular neutral camps. |
| **Camp Cleared / Populated Marker** | Shows whether a neutral camp is currently available | Can be a flip token or two-sided marker. |
| **Tower HP Marker** | Tracks current HP on each tower | Used on the shared board or shared tracking area. |
| **Tower Destroyed Marker** | Marks a destroyed tower | Large, obvious overlay marker. |
| **Barracks Status Marker** | Shows whether each Barracks is standing or destroyed | One per lane, per team. |
| **Fallen Barracks Token** | Marks a lane whose Barracks has fallen | Triggers Enhanced creeps in that lane. |
| **Mega Creeps Token** | Marks that all three Barracks have fallen for a team | Replaces per-lane Fallen Barracks tracking once Mega Creeps are active. |
| **Ancient HP Marker** | Tracks current HP on each Ancient | Shared objective tracking. |
| **Roshan HP Marker** | Tracks Roshan's current HP during fights | Can live on shared objective mat or board edge. |
| **Roshan Alive / Dead Marker** | Indicates whether Roshan is currently present | Useful between kill and respawn windows. |
| **Aegis of the Immortal Token** | Indicates the hero holding Aegis, or its dropped position on the board | One premium token. |
| **Power Rune Token** | Marks an unclaimed rune on the river | May be a generic rune token paired with rune-type determination. |
| **Rune Type Token Set** | Shows which rune is currently active or stored | Illusion, Haste, Invisibility, Regeneration, Double Damage. |
| **Courier Token** | Represents the shared team Courier on the board or tracking area | One per team. |
| **Round Start Token** | Marks the first hero in the round order | Shared rotation token. |
| **Half-Round Marker** | Marks first half vs second half of the round | Tracks forward/backward pendulum direction. |

---

## 2. Vision, Invisibility, And Deception Tokens

These tokens support the game's vision war, hidden positioning, and reveal mechanics.

| Token | Purpose | Notes |
|---|---|---|
| **Observer Ward Token** | Placed vision token that grants the tactical reaction advantage | Needs team identity and hidden/enemy-facing handling. |
| **Sentry Ward Token** | Placed true-sight token | Also hidden until revealed by enemy true sight. |
| **Ward Duration Marker** | Tracks remaining rounds on wards | Generic numeric marker preferred. |
| **Ward Revealed Marker** | Indicates a hidden ward has been exposed to the enemy | Optional helper marker if needed during playtests. |
| **Invisibility Cloud Token** | Multi-tile token hiding a single invisible hero's true position | Must support secret placement under one tile. |
| **Smoke Cloud Token** | Multi-hero hidden movement token for Smoke of Deceit | Distinct from standard invisibility cloud. |
| **Reveal Marker** | Marks temporary reveal from Dust, Sentry, or Gem coverage if needed | Optional helper token for clarity in dense fights. |
| **True Sight Aura Marker** | Optional radius helper for Gem or Sentry effects | Useful if range templates are not printed elsewhere. |

---

## 3. Planning Tokens

These are the face-down commitment tools used during the Planning Phase.

### Shared Action Tokens

| Token | Purpose |
|---|---|
| **Move** | Commit a move action |
| **Attack** | Commit a basic attack action |
| **Farm** | Commit a farm action |
| **Use Item** | Commit an item activation |
| **Pass** | Commit no further action |

### Hero-Specific Ability Tokens

Each hero needs a reusable planning token for each of their named abilities.

| Token Family | Purpose | Notes |
|---|---|---|
| **Ability 1 Token** | Commit the hero's first ability | Hero-branded token or icon treatment. |
| **Ability 2 Token** | Commit the hero's second ability | Hero-branded token or icon treatment. |
| **Ability 3 Token** | Commit the hero's third ability | Hero-branded token or icon treatment. |
| **Ultimate Token** | Commit the hero's fourth ability | Should stand out clearly from basic ability tokens. |

### Planning Requirements

- Planning token backs should be uniform where hidden information matters.
- Front faces should be icon-first, text-second.
- Hero ability tokens should share a common frame while still being hero-specific.

---

## 4. Hero Board Status And Tracking Tokens

These tokens live primarily on each player's Hero Board and track changing state.

### Status Effect Tokens

| Token | Purpose |
|---|---|
| **Stunned** | Tracks stun effects and AP loss timing |
| **Silenced** | Tracks inability to use abilities |
| **Rooted** | Tracks inability to move |
| **Slowed** | Tracks movement or AP reduction effects |
| **Invisible** | Tracks invisibility state when a full cloud token is not used |
| **Ethereal** | Tracks ethereal state |
| **Disarmed** | Tracks inability to attack |
| **Broken** | Tracks passive disable state |
| **Hexed** | Tracks polymorph / hard disable state |
| **Bleeding / DoT** | Tracks damage-over-time effects |
| **BKB Active / Spell Immunity** | Tracks temporary spell immunity or similar protection |

### Generic Tracking Markers

| Token | Purpose | Notes |
|---|---|---|
| **Duration Number Tokens** | Show remaining turns or rounds on statuses and cooldowns | Reusable numeric markers. |
| **Cooldown Tokens** | Mark abilities or items on cooldown | Can be generic or slot-specific. |
| **Ability Identifier Tokens** | Mark which hero ability is cooling down | May use Q/W/E/R style or ability icons. |
| **Channeling Token** | Marks an ability currently being channeled | Hourglass-style marker. |
| **Reaction AP Debt Token** | Tracks AP owed from reactions on the hero's next activation | Numeric marker preferred. |
| **Turn AP Spent Marker** | Tracks how much AP has been spent in the current activation | Simple cube or slider marker. |
| **Alive / Dead Flip Token** | Tracks whether the hero is alive | One per hero. |
| **Respawn Marker** | Tracks turns remaining until respawn | Numeric marker preferred. |
| **Buyback Available Marker** | Indicates whether buyback is currently available | One per hero. |
| **Buyback Cooldown / Last Used Marker** | Tracks when buyback was last used | Shared numeric marker. |
| **Level Milestone Marker** | Marks level 6, 12, and 18 unlock state | Small cube or badge marker. |
| **Scepter Acquired Token** | Marks that Aghanim's Scepter is active for the hero | One per hero. |
| **Scepter Upgrade Pointer** | Indicates which ability is upgraded if not obvious on the card | Small arrow or badge marker. |

### Stat Modification Tokens

| Token | Purpose |
|---|---|
| **+1 Attack Token** | Temporary or permanent attack increases |
| **+5 Attack Token** | Larger attack increases |
| **+10 Attack Token** | Large attack increases |
| **+1 Defense Token** | Defense increases |
| **+5 Defense Token** | Larger defense increases |
| **+1 Move Speed Token** | Move Speed increases |

---

## 5. Objective And Economy Tokens

These tokens represent globally important rewards, drops, and economy-related states.

| Token | Purpose | Notes |
|---|---|---|
| **Gold Bonus Marker** | Marks teamwide gold rewards from major objectives if needed during resolution | Optional helper token. |
| **Bottle Stored Rune Token** | Tracks which rune is currently stored in a Bottle | Uses the same rune type family where possible. |
| **Gem of True Sight Drop Token** | Marks Gem on the board after carrier death | Shared single item-drop token. |
| **Divine Rapier Drop Token** | Marks Divine Rapier on the board after carrier death | Needed if Rapier remains in final item pool. |
| **Charge Tokens** | Track charges on items such as Magic Wand, Drum, Urn, or Vessel | Reusable charge family preferred. |

---

## 6. Rune And Illusion Tokens

These tokens support temporary summoned units and rune-derived states.

| Token | Purpose | Notes |
|---|---|---|
| **Illusion Tokens** | Represent rune-, item-, or hero-generated illusions on the board | Should be visually distinct from true hero tokens. |
| **Haste Marker** | Tracks Haste rune effect on a hero | Can be a buff token on Hero Board. |
| **Invisibility Rune Marker** | Tracks Invisibility rune effect on a hero | Usually paired with cloud/invisible state handling. |
| **Regeneration Marker** | Tracks active regeneration rune effect | Useful if regen can be interrupted. |
| **Double Damage Marker** | Tracks active Double Damage buff | Strong visual priority recommended. |

---

## 7. Item Effect Tokens

These token families are referenced in the current item file and should be planned as reusable effect markers rather than one-off art pieces wherever possible.

| Token | Purpose | Source Pattern |
|---|---|---|
| **Shield Token** | Absorbs the next X incoming damage | Defensive active items |
| **Magic Barrier Token** | Absorbs the next instance of magic damage | Team defensive items |
| **Physical Block Token** | Negates the next physical damage instance | Team defensive items |
| **Static Shield Token** | Punishes the next attacker | Reactive defensive items |
| **Lotus Echo Token** | Reflects the next single-target ability | Lotus-style effects |
| **Veil Token** | Marks increased magic damage taken | Magic amplification items |
| **Nullify Token** | Marks item suppression / purge state | Offensive disable items |
| **Aeon Shield Token** | Marks temporary damage immunity trigger | Emergency defensive item |
| **Arctic Slow Token** | Marks item-applied slow and attack-speed reduction | On-hit debuff items |
| **Slow Token** | Generic movement reduction marker | Reusable across items and heroes |
| **Silence Token** | Reusable silence marker for items and hero abilities | Shared status family |
| **Hex Token** | Reusable hex marker for items and hero abilities | Shared status family |
| **Magic Damage Counter Token** | Tracks delayed damage from silence-style effects | Used when damage is calculated after the effect ends |

---

## 8. Hero-Specific Future Token Families

As more heroes are designed, some will need bespoke tokens beyond the shared status system.

Typical future examples include:
- summoned unit tokens
- trap or mine tokens
- remnant or spirit tokens
- stack counters for scaling passives
- orbiting shield or charge markers
- zone templates for persistent spell areas
- transformation state markers

These should follow one rule: if a mechanic is unique to one hero, the token should still inherit the same global icon language and production standards as the rest of the game.

---

## 9. Recommended Production Split

To keep the token system manageable, token production should be split into five manufacturing families.

| Family | Includes |
|---|---|
| **Board Presence Tokens** | Heroes, creeps, wards, rune token, courier, Roshan, dropped items |
| **Objective Tokens** | Aegis, Fallen Barracks, Mega Creeps, tower destroyed markers |
| **Planning Tokens** | Move, Attack, Farm, Use Item, Pass, hero ability tokens |
| **Status / Marker Tokens** | Stun, Silence, Root, Slow, DoT, cooldown, duration, AP debt, channeling |
| **Special Effect Tokens** | Illusions, clouds, shields, barriers, charge tokens, future hero-specific summons |

---

## 10. Minimum Prototype Token Set

If producing a first playable prototype, the minimum token set should include:

- hero tokens
- lane creep counters
- neutral and Ancient camp counters
- camp cleared markers
- tower HP and destroyed markers
- Barracks status markers
- Fallen Barracks tokens
- Mega Creeps token
- Roshan HP marker
- Aegis token
- power rune token and rune-type set
- Courier tokens
- Observer Ward and Sentry Ward tokens
- Invisibility Cloud and Smoke Cloud tokens
- Move, Attack, Farm, Use Item, Pass planning tokens
- hero-specific ability tokens for any heroes currently in the test pool
- core status tokens: Stunned, Silenced, Rooted, Slowed, DoT, Hexed, Ethereal, Disarmed
- cooldown and duration number markers
- reaction AP debt marker
- alive / dead flip tokens
- Scepter acquired marker
- charge tokens
- illusion tokens

---

## 11. Open Questions

These points should be resolved before final production art begins.

| Question | Why It Matters |
|---|---|
| Should creep representation use one wave token, multiple creep counters, or lane-specific mini-sets? | This changes both token count and board readability. |
| Should wards use hidden backs, team-only identifiers, or a referee-honour system? | Vision gameplay depends on clean hidden information handling. |
| Should rune handling use one generic rune token plus a rune die, or separate rune-face tokens? | Affects production count and usability with Bottle. |
| Should Roshan, towers, and the Ancient track HP directly on the board or on a side mat? | Determines whether more large objective markers are needed. |
| How many generic charge, duration, and cooldown markers are enough for full 5v5 play? | Necessary for punchboard planning. |
| Which future hero mechanics justify bespoke tokens instead of generic markers? | Prevents token bloat as the roster expands. |
