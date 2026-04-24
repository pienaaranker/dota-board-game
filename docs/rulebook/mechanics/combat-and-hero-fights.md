# DOTA 2: THE BOARD GAME — COMBAT AND HERO FIGHTS

This document collects combat resolution, status effects, and the shared targeting language used by hero abilities.

---

## Combat

### Damage Resolution
All combat uses the formula:

> **Damage − Defense = Health Lost**

The attacker's Damage and the defender's Defense are taken from their Hero Cards, modified by any active items and abilities.

### Line of Sight (LoS)
- **Melee Attacks** target an adjacent hex and do **not** require clear LoS.
- **Ranged Attacks and targeted Abilities** require an unobstructed line between the attacker's hex and the target's hex.
- To check LoS: draw a straight line between the two hex centres. If that line passes through any **Tree hex** or **Impassable hex**, LoS is blocked and the attack or ability cannot be used from that position.
- **AoE abilities** apply the same check per hex — only hexes with clear LoS from the caster are affected, unless the hero's Abilities Card states otherwise.

### Attack Range
- **Melee** heroes must be on a hex **adjacent** to their target to attack. No LoS required.
- **Ranged** heroes use the **attack range printed on their Hero Card** and require **clear Line of Sight** (see above).
- If a card effect changes a hero's attack range, use the modified value for as long as that effect applies.

### Status Effects

These are the default shared rules for status effects used by heroes, items, and tokens. If a card applies a status effect, it uses these rules unless that card explicitly states an exception.

| Status Effect | Mechanical Effect |
|---|---|
| **Stun** | A stun may remove **AP**, a **turn**, or a **round** as specified by the card or effect. See Stun below. |
| **Silence** | Prevents the use of abilities and interrupts channels. See Silence below. |
| **Slow** | Applies a movement AP tax for a stated number of turns or rounds. See Slow below. |
| **Root** | Stops all movement actions for the stated duration but allows other actions normally. |
| **Hex** | Prevents attacks, abilities, and item use, but leaves only extremely limited movement. |
| **Disarm** | Prevents attack actions but allows other actions normally. |
| **Break** | Disables passive abilities only. |
| **Ethereal** | Prevents normal attacks and physical weapon damage interactions. See Ethereal below. |
| **Spell Immunity** | Blocks most enemy abilities and debuffs unless an effect says it pierces spell immunity. |
| **DoT (Damage over Time)** | See DoT below. |

#### Stun

A stun removes a hero's ability to act by removing AP, a full activation, or a full round of activations.

##### Stun Timing

Stun effects use one of three measurements. The card or effect must always state which one it uses.

| Stun Type | Effect |
|---|---|
| **AP Stun** | The hero loses the stated amount of AP from their next activation. If that activation has already been planned, remove committed planning tokens from left to right until the removed tokens total at least the stun value. Those removed actions are lost. |
| **Turn Stun** | The hero loses their next activation entirely. All committed actions for that activation are lost and the hero is skipped. |
| **Round Stun** | The hero cannot act for the stated round duration. Each activation the hero would take during that round is skipped, and any committed actions for those skipped activations are lost. |

**AP stun token removal:**
- Remove tokens in committed order from left to right.
- Remove whole tokens only; do not partially reduce a token's cost.
- Continue removing tokens until the total removed AP is **equal to or greater than** the AP stun value.
- If the hero is already in the middle of an activation when the AP stun is applied, start with the next unresolved token and continue left to right through the remaining committed actions.

**Example:** A hero committed: Move (1 AP) -> Move (1 AP) -> Ability (2 AP) -> Ability (2 AP) -> Farm (2 AP) -> Farm (2 AP). If that hero is stunned for **5 AP**, remove tokens from left to right until at least 5 AP has been removed: Move (1 AP), Move (1 AP), Ability (2 AP), Ability (2 AP). The hero keeps only the two Farm actions for that activation.

#### Silence

Silence prevents a hero from using abilities for the stated duration.

**Silence rules:**
- A Silenced hero cannot activate printed hero abilities, including **Active**, **Toggle**, and **Channeled** abilities.
- Silence immediately interrupts any **Channeled** ability the hero is currently maintaining.
- A Silenced hero cannot toggle a printed hero ability on or off while Silenced.
- A Silenced hero may still move, attack, farm, and use item actions unless another effect also prevents those actions.
- Silence does not remove committed tokens in advance; ability tokens simply fail if revealed while the hero is Silenced.

#### Slow

A slow reduces how efficiently a hero can move by taxing movement AP instead of removing general AP.

##### Slow Timing

Slow effects use an **AP value** and a **duration**. The card or effect must state both.

| Slow Element | Effect |
|---|---|
| **Slow AP Value** | The first X AP spent on movement during each affected turn is lost to the slow and produces **0 hexes** of movement. |
| **Turn Duration** | The slow affects the hero for the stated number of total turns. |
| **Round Duration** | The slow affects the hero for the stated number of complete rounds. |

**Slow rules:**
- Slow affects only **Move** actions. It does not remove AP from attacks, abilities, items, or other actions.
- Slow consumes whole **Move** tokens only.
- On each affected turn, resolve the slow against the hero's movement in committed order: the first X AP worth of **Move** tokens are spent normally but move the hero **0 hexes**.
- After the slow tax has been paid for that turn, any remaining **Move** tokens work normally.
- If the hero does not use any **Move** actions on an affected turn, no AP is lost that turn, but the slow duration still decreases normally.
- If a hero is already in the middle of an activation when a slow is applied, it begins affecting the next unresolved **Move** token unless the card says it starts on the next turn or next activation instead.

**Example:** A hero is **Slowed 1 AP for 10 turns**. During each of those 10 turns, the first **Move** token the hero spends moves them **0 hexes**. If that hero wants to move **4 hexes** on one of those turns, they must commit **5 Move tokens**: 1 token to satisfy the slow, then 4 more tokens to move 4 hexes.

#### Root

Root prevents a hero from moving voluntarily for the stated duration.

**Root rules:**
- A Rooted hero cannot use **Move** actions.
- A Rooted hero may still attack, farm, use items, and use abilities unless the card or effect says otherwise.
- Root does not prevent **forced movement** caused by another hero, item, or board effect unless that effect specifically says the target cannot be moved.
- If a committed **Move** token is revealed while the hero is Rooted, that action fails normally under the failed-action rules.

#### Hex

Hex is a hard disable that shuts down a hero's actions and leaves only extremely limited movement for the stated duration.

**Hex rules:**
- A Hexed hero cannot attack, use abilities, or use items.
- A Hexed hero is treated as **Slowed 7 AP** for the duration. This is their only normal action freedom while Hexed.
- A Hexed hero's **Defense becomes 0** for the duration unless the card says otherwise.
- Hex does not remove committed tokens in advance. **Attack**, ability, and item tokens fail if revealed while the hero is Hexed. **Move** tokens are resolved using the Hex slow value.
- Forced movement may still affect a Hexed hero unless the source effect says otherwise.

#### Disarm

Disarm prevents a hero from making attack actions for the stated duration.

**Disarm rules:**
- A Disarmed hero cannot declare **Attack** actions.
- A Disarmed hero may still move, use abilities, use items, and farm unless another effect prevents those actions.
- If a committed **Attack** token is revealed while the hero is Disarmed, that action fails normally under the failed-action rules.

#### Break

Break disables passive abilities for the stated duration.

**Break rules:**
- A Broken hero gains no benefit from printed passive abilities on their Hero Card.
- Break does not affect active abilities, item abilities, or basic actions unless those abilities explicitly depend on a passive that has been disabled.
- If a passive creates a continuous bonus, that bonus is ignored while the hero is Broken.

#### Ethereal

Ethereal represents a ghostly state that shuts off normal attacking and most physical damage interactions.

**Ethereal rules:**
- An Ethereal hero cannot make **Attack** actions.
- Normal physical attack damage cannot be dealt to an Ethereal hero.
- Effects that grant bonus magic damage, extra magic vulnerability, or other ethereal modifiers must state those values on the card or item that applies Ethereal.
- Ethereal does not prevent movement or ability use unless the card says otherwise.

#### Spell Immunity

Spell Immunity protects a hero from most hostile magical interference for the stated duration.

**Spell Immunity rules:**
- Enemy abilities and debuffs cannot affect a hero with Spell Immunity unless the source explicitly says it **pierces spell immunity**.
- Spell Immunity does not prevent normal attack damage unless the card says otherwise.
- Existing dispellable debuffs on the hero are handled by the card or item granting Spell Immunity; if it also dispels, that must be stated explicitly.
- Allied abilities may still affect a Spell Immune hero if the card allows it.

#### DoT (Damage over Time)

A DoT is a debuff token placed on a hero. At the **start of that hero's activation** (when their turn begins), the DoT deals its damage and decrements its duration by 1. When the duration reaches 0, the token is removed.

**DoT rules:**
- Each DoT token specifies: damage per tick, tick frequency (every activation or every round), and total duration.
- Most DoTs tick **once per activation** — meaning twice per round since each hero activates twice.
- Some DoTs may tick **once per round** instead — this will be clearly marked on the hero's Abilities Card or the relevant item entry.
- Multiple different DoT tokens can be active on a hero simultaneously; each ticks independently.
- The same DoT type does **not** stack — applying it again refreshes the duration instead.
- Most DoTs are **dispellable**: they can be removed by items or abilities that cleanse debuffs (e.g. Eul's Scepter of Divinity, Guardian Greaves). The relevant item entry or hero's Abilities Card will state if it dispels debuffs.
- Some DoTs are marked **undispellable** on the card or item entry — these cannot be removed early.

**Named DoT types used in this game:**

| DoT Type | Damage | Frequency | Notes |
|---|---|---|---|
| **Bleed** | X physical damage | Once per activation | Applied by Blood Grenade. Dispellable. |

### Summons

Some abilities create **Summons**: controlled units that belong to a hero but are not heroes themselves.

**Core summon rules:**
- A summon is a unit on the board. It may be targeted by attacks and abilities unless the creating ability says otherwise.
- Each summon has its own mini stat line printed on the creating hero's Abilities Card or supporting component: **Hits**, **AP**, **Attack**, **Defense**, **Move Speed**, and **Mana** if relevant.
- Summon durability is tracked with **Hits**, not full HP. Each time a summon would take damage from an attack, ability, or effect that successfully affects it, it loses **1 Hit** unless the creating ability says it loses more.
- If a summon reaches **0 Hits**, remove it from the board immediately.
- Summons do not level up unless the creating ability includes scaling values.
- Unless otherwise stated, a summon cannot carry items, gain gold, collect runes, capture objectives, buy back, or use shop actions.

**Turn and activation rules:**
- A summon does not enter the round-order pendulum as a separate combatant.
- A summon acts only during its controller's activation.
- The controller may spend the summon's own AP during that activation to move, attack, or use printed summon abilities.
- Summon AP refreshes at the start of the controller's activation, not at the start of every turn on the table.
- Unless otherwise stated, each summon may take the shared actions **Move**, **Attack**, and **Pass**.

**Board and control rules:**
- Summons count as allied units for auras, targeting, blocking movement, and occupying hexes.
- A summon occupies its own hex and follows the same terrain and Line of Sight rules as other units unless the creating ability says otherwise.
- If the controlling hero dies, remove that hero's summons immediately unless a specific ability says they persist.
- If multiple summons are created by one ability, each summon tracks its own remaining Hits, but matching summons may share the same printed stat line.

**Summon timing and bookkeeping:**
- Summons with a limited duration are removed when that duration expires, even if they still have Hits remaining.
- If a summon has Mana, that Mana is tracked separately from the hero's Mana.
- If a summon applies a repeated debuff such as armor reduction, use shared status or modifier tokens where possible instead of bespoke markers.

### Death
When a hero's Health reaches 0 they are removed from the board and enter a respawn countdown (see Economy and Progression).

---

## Ability Types & Targeting

Hero abilities use different targeting and activation methods. This section defines how each type works in the board game context. All entries are pending design discussion.

### Activation Methods

**Passive** — Always active; no mana cost or activation required. Effect is continuous as long as the hero is alive.

**Active** — Manually cast during a hero's turn. Costs Mana and AP as printed on the hero's Abilities Card.

**Toggle** — Can only be **activated** during the hero's own turn (costs Mana and AP as printed). Once active, can be **toggled off at any time** — even during another player's turn — unless the hero is Silenced. While the hero is Silenced, the toggle remains in its current state and cannot be switched on or off. While active, may drain Mana or Health per round. Examples: Rot, Mana Shield.

**Channeled** — Can be **activated** during the hero's own turn (costs Mana and AP as printed on the hero's Abilities Card). Once active, the hero must remain stationary and the effect persists across subsequent turns until interrupted or cancelled. **Interrupted by:** Stun, Silence, forced movement, or the target moving out of range. The casting player may **cancel the channel at any time** (like a toggle). Examples: Freezing Field, Black Hole.

### Targeting Types

**No Target (Self-Cast)** — Instant effect centered on or affecting only the caster. No targeting step required. Examples: God's Strength, Battle Hunger.

**Unit Target (Single Target)** — Targets a specific unit (ally, enemy, creep, or structure) within range and LoS. Must declare target before resolving.

**Point Target** — Player declares a specific hex within range as the target location. The effect occurs at that hex. Whether the effect is instant or has travel time is specified on the hero's Abilities Card. Examples: Light Strike Array, Ice Path.

**Direction/Vector Target** — Player declares a direction or line from the caster by specifying a target hex. How the ability resolves along that direction (instant movement, projectile, persistent zone, etc.) is specified on the hero's Abilities Card. Examples: Swashbuckle (movement + attack along direction), Macropyre (line of fire).

### Effect Shapes

**Circular AoE** — Affects all units within a fixed radius (measured in hexes) from the center point.

**Linear/Line** — Straight line from caster extending outward. Hits all units along the path.

**Cone** — Wedge-shaped area in front of the caster. Hits all units in the cone.

**Global** — Affects all enemy or allied heroes (as specified on the card) on the entire board, regardless of range or Line of Sight. No targeting step required — all valid targets are affected simultaneously. Balance is handled through the ability's damage values, mana cost, cooldown, and other printed parameters. Examples: Thundergod's Wrath, Nature's Call.

### Special Mechanics

**Skillshot** — Abilities that travel in a line from the caster to a target location and can be dodged. **Whether an ability is a skillshot must be explicitly marked on the hero's Abilities Card.** Only abilities marked as Skillshot may be dodged using the Dodge Skillshot reaction — all other abilities resolve instantly and too quickly to dodge. The caster declares a direction by specifying a target hex (using Direction/Vector targeting). The ability creates a line effect from the caster's hex toward the target hex. Any hero in the path of the skillshot (including at the end position) may use the **Dodge Skillshot** reaction (see Turn Structure) to attempt to avoid being hit. The dodge reaction costs 2 AP from the hero's next turn, requires a die roll to determine success, and forces the hero to immediately move to an adjacent hex regardless of the roll's outcome. Examples: Sacred Arrow, Meat Hook.

**Ground-Targeted AoE** — Combination of Point Target + Circular AoE. Player picks a hex; all units within the radius are affected.

**Unit-Targeted AoE** — Targets a unit; effect radiates from that unit to nearby hexes. Examples: Poison Nova, Thundergod's Wrath (per-hero basis).

**Aura** — Passive effect that continuously radiates from the hero to all allied or enemy units (as specified on the card) within a fixed range measured in hexes. The aura's radius, which units are affected (allies/enemies/both), and the specific effect are all printed on the hero's Abilities Card. Auras are always active while the hero is alive and do not require activation. Examples: Precision Aura, Vampiric Aura.
