# Token Amounts

This file is the pragmatic count sheet for physical tokens.

## Shape System

Use a small shared shape language so token families are easy to sort at a glance during play and easy to lay out for print production.

- **Hex** = board-state and map-presence tokens that live directly on hex spaces
- **Diamond** = planning and commitment tokens
- **Circle** = premium objective or unique state markers
- **Custom Template** = non-standard hidden-position pieces that need their own footprint

## Planning Token Compression Rule

To reduce token count, repeatable planning actions can use **denomination tokens** instead of one token per action.

- **1** = one consecutive use of that action
- **3** = three consecutive uses of that action
- **5** = five consecutive uses of that action

This only works as a shorthand for **consecutive identical queued actions**. If a player wants to plan `Move -> Attack -> Move`, those must still be represented as separate queued commitments.

---

## Board Presence And Objective Tokens

| Token | Amount | Shape | Notes |
|---|---:|---|---|
| Lane Creep Tokens | 6 | Hex | One wave token per side per lane. |
| Neutral Camp Tokens | 8 | Hex | 4 regular neutral camps per side. |
| Ancient Camp Tokens | 2 | Hex | 1 Ancient camp per side. |
| Ancient Marker | 0 | Hex | Ancient should be printed on the board, not tracked with a token. |
| Tower Marker | 0 | Hex | Tower positions should be printed on the board. Use destroyed markers separately if needed. |
| Barracks Status Marker | 6 | Hex | 3 Barracks per side. |
| Roshan Marker | 1 | Circle | One Roshan state piece. |
| Aegis of the Immortal Token | 1 | Circle | One premium objective token. |
| Power Rune Tokens | 5 | Hex | One for each rune type. |
| Courier Tokens | 2 | Hex | One Courier per team. |
| Broken Tree Tokens | 20 | Hex | Practical prototype count, not a hard maximum. |

## Vision, Hidden Information, And Deception Tokens

| Token | Amount | Shape | Notes |
|---|---:|---|---|
| Observer Ward Tokens | 12 | Hex | Supports up to 6 active wards per team. |
| Sentry Ward Tokens | 12 | Hex | Supports up to 6 active wards per team. |
| Invisibility Cloud Tokens | 10 | Custom Template | Enough for all 10 heroes to be invisible at once. |
| Smoke Cloud Tokens | 2 | Custom Template | One active Smoke group per team is a practical ceiling. |

## Shared Planning Tokens

For a 10-hero game, these counts assume compressed denomination tokens instead of one token per action.

### Move Tokens

| Token | Amount | Shape | Notes |
|---|---:|---|---|
| Move 1 Hex | 20 | Diamond | Fine-grain queue control. |
| Move 3 Hexes | 10 | Diamond | Covers common travel bursts. |
| Move 5 Hexes | 10 | Diamond | Covers long repeated movement queues. |

### Attack Tokens

| Token | Amount | Shape | Notes |
|---|---:|---|---|
| Attack x1 | 40 | Diamond | Single committed attacks. |

### Item Slot Tokens

| Token | Amount | Shape | Notes |
|---|---:|---|---|
| Item Slot 1 Token | 10 | Diamond | One per hero. |
| Item Slot 2 Token | 10 | Diamond | One per hero. |
| Item Slot 3 Token | 10 | Diamond | One per hero. |
| Item Slot 4 Token | 10 | Diamond | One per hero. |
| Item Slot 5 Token | 10 | Diamond | One per hero. |
| Item Slot 6 Token | 10 | Diamond | One per hero. |

## Hero Ability Planning Tokens

These are still best kept at one per hero per slot, because they refer to distinct named abilities rather than generic repeatable actions.

| Token | Amount | Shape | Notes |
|---|---:|---|---|
| Ability 1 Token | 10 | Diamond | One per hero in a 10-hero game. |
| Ability 2 Token | 10 | Diamond | One per hero in a 10-hero game. |
| Ability 3 Token | 10 | Diamond | One per hero in a 10-hero game. |
| Ultimate Token | 10 | Diamond | One per hero in a 10-hero game. |
| Rubick Stolen Spell 1 Token | 1 | Diamond | Only needed if Rubick is in the game. |
| Rubick Stolen Spell 2 Token | 1 | Diamond | Only needed if Rubick is in the game. |
| Invoker Invoked Spell 1 Token | 1 | Diamond | Only needed if Invoker is in the game. |
| Invoker Invoked Spell 2 Token | 1 | Diamond | Only needed if Invoker is in the game. |

## Status And State Tokens

These are practical prototype counts for shared debuffs and hero-board state markers. Using 5 copies of each shared status keeps the full family slightly above the `50+` status-token target in the hero-board layout notes once Buyback tokens are included.

| Token | Amount | Shape | Notes |
|---|---:|---|---|
| Stunned | 5 | Circle | Practical shared pool for simultaneous disables across both teams. |
| Silenced | 5 | Circle | Practical shared pool for simultaneous disables across both teams. |
| Rooted | 5 | Circle | Practical shared pool for simultaneous disables across both teams. |
| Slowed | 5 | Circle | Practical shared pool for simultaneous movement debuffs across both teams. |
| Ethereal | 5 | Circle | Practical shared pool for temporary state changes across both teams. |
| Disarmed | 5 | Circle | Practical shared pool for simultaneous disables across both teams. |
| Broken | 5 | Circle | Practical shared pool for passive-disable effects across both teams. |
| Hexed | 5 | Circle | Practical shared pool for simultaneous hard disables across both teams. |
| DoT | 5 | Circle | Practical shared pool for bleed, burn, and other damage-over-time effects. |
| Buyback Token | 10 | Circle | One per hero in a 10-hero game. |

## Current Hero-Specific Effect Tokens

| Token | Amount | Shape | Notes |
|---|---:|---|---|
| Healing Ward Token | 1 | Hex | Juggernaut can have only one Healing Ward on the board at a time. |
| Weaver Swarm Beetle Token | 5 | Circle | Supports marking every enemy hero on one team at once. |
| Weaver Time Lapse Marker | 1 | Hex | Weaver tracks one saved rewind position at a time. |
| Rubick Spell Steal Marker Token | 2 | Circle | Rubick has 1 by default; a second becomes usable with Aghanim's Scepter. |
| Rubick Spell Steal Cooldown Token | 1 | Circle | Rubick has one dedicated Spell Steal cooldown identity marker. |
| Invoker Orb Token | 3 | Circle | Invoker always has exactly 3 active orb slots. |
| Invoker Invoke Slot Marker | 2 | Circle | Invoker has 2 Invoke Slots. |
| EMP Charge Token | 1 | Hex | EMP uses one delayed-resolution target marker at a time. |
| Forge Spirit Token | 2 | Hex | Invoker can have 2 Forge Spirits in play at level 12+. |
| Invoker Forge Spirit Armor Break Marker | 5 | Circle | Supports tracking the debuff on multiple enemy heroes at once. |

## Conditional Or Optional Current-File Tokens

| Token | Amount | Shape | Notes |
|---|---:|---|---|
| Gem of True Sight Drop Token | 1 | Hex | Only needed if Gem remains a droppable board item. |
| Divine Rapier Drop Token | 1 | Hex | Only needed if Divine Rapier remains in the final item pool. |
